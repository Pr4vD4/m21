<template>
  <route-main />
  <div class="about">
    <h1>This is an about page</h1>
  </div>
  <click-button />
</template>
<script>
import RouteMain from "@/components/nav/RouteMain";
import ClickButton from "@/components/forms/ClickButton";
export default {
  components: { RouteMain, ClickButton },
};
</script>
