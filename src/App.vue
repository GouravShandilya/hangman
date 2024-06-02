<template>
  <!-- <div id="app">hi rahul</div> -->
  <!-- <Login /> -->
  <LandingPage />
</template>
<script>
// import Login from "./components/User/Login.vue";
import LandingPage from "./components/LnadingPage/index.vue";
export default {
  name: "App",
  components: { LandingPage },
};
</script>
<style lang="scss">
* {
  padding: 0%;
  margin: 0%;
  box-sizing: border-box;
}
body {
  font-family: sans-serif;
  // background-color: wh;
  background: rgb(226, 193, 232);
  background: linear-gradient(
    90deg,
    rgba(226, 193, 232, 1) 0%,
    rgba(210, 222, 222, 1) 19%,
    rgba(241, 241, 241, 1) 100%
  );
}
</style>
