<template>
  <div>
    <el-collapse accordion>
      <el-collapse-item title="行属性" name="1">
        <table>
          <thead>
            <tr>
              <th>参数</th>
              <th>说明</th>
              <th>类型</th>
              <th>可选值</th>
              <th>默认值</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>gutter</td>
              <td>栅格间隔</td>
              <td>number</td>
              <td>—</td>
              <td>0</td>
            </tr>
            <tr>
              <td>type</td>
              <td>布局模式，可选 flex，现代浏览器下有效</td>
              <td>string</td>
              <td>—</td>
              <td>—</td>
            </tr>
            <tr>
              <td>justify</td>
              <td>flex 布局下的水平排列方式</td>
              <td>string</td>
              <td>start/end/center/space-around/space-between</td>
              <td>start</td>
            </tr>
            <tr>
              <td>align</td>
              <td>flex 布局下的垂直排列方式</td>
              <td>string</td>
              <td>top/middle/bottom</td>
              <td>top</td>
            </tr>
            <tr>
              <td>tag</td>
              <td>自定义元素标签</td>
              <td>string</td>
              <td>*</td>
              <td>div</td>
            </tr>
          </tbody>
        </table>
      </el-collapse-item>
      <el-collapse-item title="列属性" name="2">
        <table>
          <thead>
            <tr>
              <th>参数</th>
              <th>说明</th>
              <th>类型</th>
              <th>可选值</th>
              <th>默认值</th>
            </tr>
          </thead>
          <tbody>
            <tr>
              <td>span</td>
              <td>栅格占据的列数</td>
              <td>number</td>
              <td>—</td>
              <td>24</td>
            </tr>
            <tr>
              <td>offset</td>
              <td>栅格左侧的间隔格数</td>
              <td>number</td>
              <td>—</td>
              <td>0</td>
            </tr>
            <tr>
              <td>push</td>
              <td>栅格向右移动格数</td>
              <td>number</td>
              <td>—</td>
              <td>0</td>
            </tr>
            <tr>
              <td>pull</td>
              <td>栅格向左移动格数</td>
              <td>number</td>
              <td>—</td>
              <td>0</td>
            </tr>
            <tr>
              <td>xs</td>
              <td>
                <code>&lt;768px</code> 响应式栅格数或者栅格属性对象
              </td>
              <td>number/object (例如： {span: 4, offset: 4})</td>
              <td>—</td>
              <td>—</td>
            </tr>
            <tr>
              <td>sm</td>
              <td>
                <code>≥768px</code> 响应式栅格数或者栅格属性对象
              </td>
              <td>number/object (例如： {span: 4, offset: 4})</td>
              <td>—</td>
              <td>—</td>
            </tr>
            <tr>
              <td>md</td>
              <td>
                <code>≥992px</code> 响应式栅格数或者栅格属性对象
              </td>
              <td>number/object (例如： {span: 4, offset: 4})</td>
              <td>—</td>
              <td>—</td>
            </tr>
            <tr>
              <td>lg</td>
              <td>
                <code>≥1200px</code> 响应式栅格数或者栅格属性对象
              </td>
              <td>number/object (例如： {span: 4, offset: 4})</td>
              <td>—</td>
              <td>—</td>
            </tr>
            <tr>
              <td>xl</td>
              <td>
                <code>≥1920px</code> 响应式栅格数或者栅格属性对象
              </td>
              <td>number/object (例如： {span: 4, offset: 4})</td>
              <td>—</td>
              <td>—</td>
            </tr>
            <tr>
              <td>tag</td>
              <td>自定义元素标签</td>
              <td>string</td>
              <td>*</td>
              <td>div</td>
            </tr>
          </tbody>
        </table>
      </el-collapse-item>
    </el-collapse>
  </div>
</template>

<script>
export default {};
</script>
