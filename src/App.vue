<template>
  <HelloWorld />
  <!-- <Signin /> -->
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
// import Signin from "./components/Signin.vue";
export default {
  name: "App",
  components: {
    HelloWorld,
    // Signin,
  },
};
</script>

<style lang="scss">
@import "~@/../mdb/scss/index.free.scss";

#app {
  font-family: Roboto, Helvetica, Arial, sans-serif;
}
</style>
