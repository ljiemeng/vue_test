<!--
 * @Date: 2025-08-20 00:48:18
 * @LastEditTime: 2025-08-20 00:55:20
 * @Author: wangyongjie
 * @Note:  
-->
<template>
  <div>
    <h2>{{ message }}</h2>
    <h2 class="title" @click="showName">学生名称：{{ name }}</h2>
    <h2>学生年龄：{{ age + 1 }}</h2>
    <h2>学生性别：{{ sex }}</h2>
  </div>
</template>

<script>
import { myMixin } from "../mixin.js";
export default {
  name: "StudentInfo",
  data() {
    return {
      message: "你好啊，欢迎来到这里学习！！！",
      name: "张三",
      age: 18,
      sex: "男",
    };
  },
  mixins: [myMixin],
};
</script>

<style>
.title {
  color: red;
}
</style>
