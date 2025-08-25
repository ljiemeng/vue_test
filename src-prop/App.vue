<template>
  <div id="app">
    <StudentInfo name="小刘" :age="18" sex="男" />
  </div>
</template>

<script>
import StudentInfo from "./components/StudentInfo.vue";

export default {
  name: "App",
  components: {
    StudentInfo,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
