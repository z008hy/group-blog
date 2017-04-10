<template>
  <el-row :gutter="20">
    <el-col :span="20" :offset="2">
      <h3>最新资源</h3>
      <el-table :data="resourcesTableData" border style="width: 100%">
        <el-table-column label="资源类型">
          <template scope="scope">
            <span>{{ scope.row.type }}</span>
          </template>
        </el-table-column>
        <el-table-column label="更新日期">
          <template scope="scope">
            <el-icon name="time"></el-icon>
            <span>{{ scope.row.date }}</span>
          </template>
        </el-table-column>
        <el-table-column label="资源描述">
          <template scope="scope">
            <span>{{ scope.row.description }}</span>
          </template>
        </el-table-column>
        <el-table-column label="资源链接">
          <template scope="scope">
            <span>{{ scope.row.link }}</span>
          </template>
        </el-table-column>
        <el-table-column label="资源密码">
          <template scope="scope">
            <span>{{ scope.row.password }}</span>
          </template>
        </el-table-column>
      </el-table>
    </el-col>
  </el-row>
</template>

<script>
  export default {
    data() {
      return {
        resourcesTableData: [
          { date: '20170410', type: '百度云', description: 'NodeJs+JavaScript视频教程', link: 'http://pan.baidu.com/s/1sjQPDrn', password: 'a54k' },
          { date: '20170410', type: '百度云', description: 'Node.js 4.x 入门实战视频课程', link: 'http://pan.baidu.com/s/1c2ADcLa', password: 'rkwe' },
          { date: '20170410', type: '百度云', description: 'Node.js 4.x 核心技术之 Buffer精通', link: 'http://pan.baidu.com/s/1i5C4H8p', password: 'cv71' },
          { date: '20170410', type: '百度云', description: 'Node.js - Express 4.x框架高级实战', link: 'http://pan.baidu.com/s/1o8AY9V8', password: 'ens8' },
        ],
      };
    },
  };
</script>
