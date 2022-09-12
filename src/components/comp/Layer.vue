<template>
  <div class="d-flex">
    <select class="form-select select bg" aria-label="Default select example">
      <option selected>Open this select menu</option>
      <option value="bg-dark">dark</option>
      <option value="2">Two</option>
      <option value="3">Three</option>
    </select>
    <span class="bg-primary"></span>
  </div>
</template>

<script>
export default {
  name: `Layer`,
};
</script>

<style scoped>
span {
  padding: 10px 100px;
  border-radius: 5px;
}
.select {
  width: 200px;
}
</style>
