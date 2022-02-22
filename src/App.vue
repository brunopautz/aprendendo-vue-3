<template>
  <PrimeiroComponente />
  <LyfeCyde />
  <Pessoa />

</template>

<script>

  import PrimeiroComponente from './components/PrimeiroComponente.vue'
  import LyfeCyde from './components/LyfeCyde.vue'
  import Pessoa from './components/Pessoa.vue'



  export default {
    name: 'App',
    components: {
      PrimeiroComponente,
      LyfeCyde,
      Pessoa
    }
  }
</script>
