<template>
    <div class="contents">
      <el-row :gutter="20">
        <el-col :span="12"><div class="content1"><Status></Status></div></el-col>
        <el-col :span="12"><div class="content1"><todo-list /></div> </el-col>
      </el-row>   
    </div>
</template>

<script>
import Status from './status/index.vue'
import TodoList from './TodoList/index.vue'
export default {
  name: 'TextContent',
  components:{
    Status,
    TodoList
  }
};
</script>

<style scoped>
.contents {
  margin-top: 40px;
  box-sizing: border-box;
  background-color: #eeeff2;
  border-radius: 5px;
}
.content1:hover {
  box-shadow: 0 0 10px rgba(179, 177, 177, 0.45);
}
.content1{
  background-color: #fff;
  border-radius: 5px;
}
</style>