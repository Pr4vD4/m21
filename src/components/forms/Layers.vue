<template>
  <div>
    <div class="mb-3">
      <label for="exampleInputEmail1" class="form-label">kolvo</label>
      <input type="number" v-model="amountOfLayers" />
    </div>
    <span v-for="n in +amountOfLayers" :key="n">{{ n }}</span>
  </div>
  <div class="d-felx">
    <div class="layers">
      <layer v-for="i in +amountOfLayers" :key="i" :amount-of-layers="[amountOfLayers]" />
    </div>
  </div>
</template>

<script>
import Layer from "@/components/comp/Layer";
export default {
  name: `Layers`,
  components: { Layer },
  data() {
    return {
      amountOfLayers: "",
    };
  },

};
</script>

<style scoped>
.layers div {
  margin: 20px;
}
</style>
