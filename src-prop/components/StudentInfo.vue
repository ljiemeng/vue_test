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
export default {
  name: "StudentInfo",
  data() {
    return {
      message: "你好啊，欢迎来到这里学习！！！",
    };
  },
  methods: {
    showName() {
      alert(this.name);
    },
  },
  // 谨记：props是只读的，不能修改，若要修改，需要赋值给data，通过data来修改！！！！
  // 接收父组件传递过来的数据 --第一种写法：简写形式
  // props: ["name", "age", "sex"],
  // 接收父组件传递过来的数据 --第二种写法：完整写法,定义了数据类型
  // props: {
  //   name: String,
  //   age: Number,
  //   sex: String,
  // },
  // 接收父组件传递过来的数据 --第三种写法：定义了数据类型，并且指定了默认值
  props: {
    name: {
      type: String,
      required: true,
    },
    age: {
      type: Number,
      default: 18,
    },
    sex: {
      type: String,
      default: "男",
    },
  },
};
</script>

<style>
.title {
  color: red;
}
</style>
