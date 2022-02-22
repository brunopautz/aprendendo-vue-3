<template>
  <div>
    <Header />
    <PrimeiroComponente />
    <LyfeCyde />
    <Pessoa />
  </div>
</template>

<script>

  import Header from './components/Header.vue'
  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LyfeCyde from './components/LyfeCyde.vue'
  import Pessoa from './components/Pessoa.vue'
  export default {
    name: 'App',
    components: {
      Header,
      PrimeiroComponente,
      LyfeCyde,
      Pessoa
    }
  }
</script>


<style>
  body {
    background-color: #333;
    color: #fff;
  }

  a {
    color: red;
  }
</style>