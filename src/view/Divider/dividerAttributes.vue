<template>
    <div>
        <el-collapse>
            <el-collapse-item title="属性">
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
                            <td>direction</td>
                            <td>设置分割线方向</td>
                            <td>string</td>
                            <td>horizontal / vertical</td>
                            <td>horizontal</td>
                        </tr>
                        <tr>
                            <td>content-position</td>
                            <td>设置分割线文案的位置</td>
                            <td>string</td>
                            <td>left / right / center</td>
                            <td>center</td>
                        </tr>
                    </tbody>
                </table>
            </el-collapse-item>
        </el-collapse>
    </div>
</template>


