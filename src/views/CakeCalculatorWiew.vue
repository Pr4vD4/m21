<template>
  <route-main />
  <layers />
  <div class="container d-flex"></div>
</template>

<script>
import RouteMain from "@/components/nav/RouteMain";
import Layers from "@/components/forms/Layers";
export default {
  name: "CakeCalculatorWiew",
  components: { RouteMain, Layers },
};
</script>

<style scoped></style>
