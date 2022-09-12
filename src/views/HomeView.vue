<template>
  <div class="home">
    <route-main />
    <img alt="Vue logo" src="../assets/logo.png" />
    <HelloWorld msg="Welcome to Your Vue.js App" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from "@/components/HelloWorld.vue";
import RouteMain from "@/components/nav/RouteMain";

export default {
  components: {
    HelloWorld,
    RouteMain,
  },
};
</script>
