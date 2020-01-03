<template>
  <div>
    <!-- 按钮 -->
    <el-button type="success" size="small" @click="toAddHandler">添加</el-button> 
    <el-button type="danger" size="small">批量删除</el-button>
    <!-- /按钮 -->
    <el-table :data="product">
      <el-table-column prop="id" label="编号"></el-table-column>
      <el-table-column prop="name" label="产品名称"></el-table-column>
      <el-table-column prop="price" label="价格"></el-table-column>
      <el-table-column prop="description" label="描述"></el-table-column>
      <el-table-column prop="categoryId" label="所属产品"></el-table-column>

      <el-table-column label="操作">
        <template v-slot="slot">
          <a href="" @click.prevent="toDeleteHandler(slot.row.id)">详情</a>
        
        </template>
      </el-table-column>
    </el-table>
    </div>
</template>
<script>
</script>

<style scoped>
 
</style>