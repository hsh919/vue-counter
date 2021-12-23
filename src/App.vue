<template>
  <div id="app">
    <h1>{{ count }}</h1>
    <button class="btn btn-danger" @click="decrease">–</button>
    <button class="btn btn-info mx-1" @click="reset">reset</button>
    <button class="btn btn-success" @click="increase">+</button>
  </div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return { count: 0 };
  },
  methods: {
    increase() {
      this.count++;
    },
    decrease() {
      this.count--;
    },
    reset() {
      this.count = 0;
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.btn {
  font-size: 30px;
  font-weight: bold;
}
</style>
