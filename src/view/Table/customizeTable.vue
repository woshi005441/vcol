<template>
<div>
    <el-table :data="tableData" style="width: 100%">
        <el-table-column label="日期" width="180">
            <template slot-scope="scope">
                <i class="el-icon-time"></i>
                <span style="margin-left: 10px">{{ scope.row.date }}</span>
            </template>
        </el-table-column>
        <el-table-column label="姓名" width="180">
            <template slot-scope="scope">
                <el-popover trigger="hover" placement="top">
                    <p>姓名: {{ scope.row.name }}</p>
                    <p>住址: {{ scope.row.address }}</p>
                    <div slot="reference" class="name-wrapper">
                        <el-tag size="medium">{{ scope.row.name }}</el-tag>
                    </div>
                </el-popover>
            </template>
        </el-table-column>
        <el-table-column label="操作">
            <template slot-scope="scope">
                <el-button size="mini" @click="handleEdit(scope.$index, scope.row)">编辑</el-button>
                <el-button size="mini" type="danger" @click="handleDelete(scope.$index, scope.row)">删除</el-button>
            </template>
        </el-table-column>
    </el-table>
    <p>通过 <code>Scoped slot</code> 可以获取到 row, column, $index 和 store（table 内部的状态管理）的数据</p>
    <el-collapse>
        <el-collapse-item title="显示代码" name="1">
            <el-input type="textarea" :autosize="{ minRows: 25, maxRows: 4}" readonly placeholder="请输入内容" v-model="textarea2"></el-input>
        </el-collapse-item>
    </el-collapse>
</div>
</template>

<script>
    export default {
        data() {
            return {
                textarea2: `
                <template>
                    <div>
                        <el-table :data="tableData" style="width: 100%">
                          <el-table-column label="日期" width="180">
                              <template slot-scope="scope">
                                  <i class="el-icon-time"></i>
                                  <span style="margin-left: 10px">{{ scope.row.date }}</span>
                              </template>
                          </el-table-column>
                          <el-table-column label="姓名" width="180">
                              <template slot-scope="scope">
                                  <el-popover trigger="hover" placement="top">
                                      <p>姓名: {{ scope.row.name }}</p>
                                      <p>住址: {{ scope.row.address }}</p>
                                      <div slot="reference" class="name-wrapper">
                                          <el-tag size="medium">{{ scope.row.name }}</el-tag>
                                      </div>
                                  </el-popover>
                              </template>
                          </el-table-column>
                          <el-table-column label="操作">
                              <template slot-scope="scope">
                                  <el-button size="mini" @click="handleEdit(scope.$index, scope.row)">编辑</el-button>
                                  <el-button size="mini" type="danger" @click="handleDelete(scope.$index, scope.row)">删除</el-button>
                              </template>
                          </el-table-column>
                      </el-table>
                    </div>
                  </template>
            `,
      tableData: [{
          date: '2016-05-02',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1518 弄',
          tag: '家'
        }, {
          date: '2016-05-04',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1517 弄',
          tag: '公司'
        }, {
          date: '2016-05-01',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1519 弄',
          tag: '家'
        }, {
          date: '2016-05-03',
          name: '王小虎',
          address: '上海市普陀区金沙江路 1516 弄',
          tag: '公司'
        }]
    };
  },
  methods: {
    handleEdit(index, row) {
        console.log(index, row);
      },
      handleDelete(index, row) {
        console.log(index, row);
      }
  }
};
</script>
