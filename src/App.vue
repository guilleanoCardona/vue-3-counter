<script>
export default {
  data() {
    return {
      contador: 0,
    };
  },
  methods: {
    incrementar() {
      this.contador++;
    },
    decrementar() {
      this.contador--;
    },
    reset() {
      this.contador = 0;
    },
  },
};
</script>
<template>
  <div class="container">
    <img src="./assets/logo.svg" width="125" height="125" alt="Logo Vue" />
    <small>
      <h1>Welcome to the VueJs3</h1>
    </small>
    <hr />
    <h2>Contador: {{ contador }}</h2>
    <button @click="incrementar">+1</button>
    <button @click="decrementar">-1</button>
    <button @click="reset">Reset</button>
  </div>
</template>
<style scoped>
.container {
  text-align: center;
}
h1 {
  font-weight: bolder;
  color: #667;
}
h2 {
  font-size: 2.5rem;
}
button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0 6px;
}
</style>
