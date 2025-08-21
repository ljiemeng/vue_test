<!--
 * @Date: 2025-08-20 00:48:18
 * @LastEditTime: 2025-08-20 00:55:20
 * @Author: wangyongjie
 * @Note:  
-->
<template>
  <div>
    <h2 class="title">学生名称：{{ name }}</h2>
    <h2>学生年龄：{{ age }}</h2>
  </div>
</template>

<script>
export default {
  name: "StudentInfo",
  data() {
    return {
      name: "小张",
      age: 23,
    };
  },
};
</script>

<style>
.title {
  color: red;
}
</style>
