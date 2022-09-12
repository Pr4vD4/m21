<template>
  <route-main />
  <div class="contacts">
    <h1>This is an contacts page</h1>
  </div>
  <click-button />
</template>

<script>
import RouteMain from "@/components/nav/RouteMain";
import ClickButton from "@/components/forms/ClickButton";

export default {
  name: "ContactsWiew",
  components: { RouteMain, ClickButton },
};
</script>

<style scoped></style>
