<template>
  <div class="about">
    <h1>This is about page</h1>
    <Signin />
  </div>
</template>

<script>
// @ is an alias to /src
import Signin from "@/components/Signin.vue";

export default {
  name: "About",
  components: {
    Signin,
  },
};
</script>
