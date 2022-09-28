<template>
  <div class="d-flex">
    <select class="form-select select bg" v-model.number="select" @change="count(amountOfLayers)">
      <option v-for="option in options" :key="option" :value="option">{{ option.name }}</option>
    </select>
    <span v-bind:class="[ select.color ]">Price: {{ select.price }}</span>
  </div>
</template>

<script>
export default {
  name: `Layer`,
  props: {amountOfLayers: Array},
  data() {
    return {
      select: {color: "bg-primary", price: "Выберете параметр"},
      options: [
        {color: "bg-warning", price: 100, name: "Nut"},
        {color: "bg-dark", price: 480, name: "Chocolate"},
        {color: "bg-light dark-font", price: 320, name:"Cream"}
      ]
    }
  },
  methods: {
    count(value){
      for (let i = 0; i < value; i++) {
        console.log("hello")
      }
    }
  },
};
</script>

<style scoped>
span {
  color: white;
  padding: 10px 100px;
  border-radius: 5px;
}
.select {
  width: 200px;
}
.dark-font {
  color: black;
}
</style>
