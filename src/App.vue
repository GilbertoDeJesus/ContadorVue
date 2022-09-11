<script>
export default {
  data: () => ({
    contador: 500,
  }),
  methods: {
    saludar() {
      console.log("Hola 10A");
    },
    incrementar() {
      this.contador++;
    },
    decrementar() {
      this.contador--;
    },
    resetear() {
      this.contador = 500;
    }
  }
};
</script>

<template>
  <nav class="navbar navbar-expand-lg fixed-top navbar-light bg-light mb-4">
    <h2 class="text-success">Gilberto Angel de Jesus Suarez | 10° A DGS</h2>
  </nav>
  <div class="container">
    <img src="./assets/logo.svg" alt="Logo VUE" width="125" height="125">
    <small>
      <h1>Hola desde VUE.js 3</h1>
    </small>
    <hr>
    <h2>Contador {{ contador }}</h2>
    <button @click="incrementar()">+1</button>
    <button @click="decrementar()">-1</button>
    <button @click="resetear()">Reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
  padding-top: 4rem;
}

small {
  color: #666;
}

h1 {
  font-weight: bolder;
}

h2 {
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 1.25rem;
  margin: 0px 8px;
  border: 1px solid gray;
  border-radius: 3px;
}
</style>