<!--
 * @Date: 2025-08-20 00:48:18
 * @LastEditTime: 2025-08-20 00:58:12
 * @Author: wangyongjie
 * @Note:  
-->
<template>
  <div>
    <h2>学校名称：{{ name }}</h2>
    <h2>学校地址：{{ address }}</h2>
    <button @click="showSchoolName">点我提示学校名</button>
  </div>
</template>

<script>
export default {
  name: "SchoolInfo",
  data() {
    return {
      name: "尚硅谷",
      address: "北京-昌平",
    };
  },
  methods: {
    showSchoolName() {
      alert(this.schoolName);
    },
  },
};
</script>
