<template>
  <!--  <div class="form">
    <form action="" id="form1">
      <label>Wanna click&<button>Click!</button></label>
    </form>
  </div>-->

  <div id="example-1">
    <button @click="inc">+1</button>
    <button @click="clear">-</button>
    <p>Кнопка выше была нажата {{ counter }} раз</p>
  </div>
</template>

<script>
export default {
  name: "ClickButton",
  data() {
    return {
      counter: 0,
      counterKey: "counter",
    };
  },
  methods: {
    inc() {
      this.counter += 1;
    },
    clear() {
      this.counter = 0;
    },
    getLocalStorage(key) {
      return localStorage.getItem(key);
    },
    setLocalStorage(key, value) {
      localStorage.setItem(key, value);
    },
  },
  watch: {
    counter(value) {
      this.setLocalStorage(this.counterKey, value);
    },
  },
  mounted() {
    this.counter = +this.getLocalStorage(this.counterKey);
  },
};
</script>

<style scoped>
button {
  padding: 0.2rem 0.4rem;
  font-size: 1.1rem;
  font-family: Calibri;
  background: lightskyblue;
  border: none;
  box-shadow: 0.1rem 0.1rem 2px 1px cornflowerblue;
}
button:active {
  box-shadow: 0.18rem 0.18rem 4px 2px blue;
}
</style>
