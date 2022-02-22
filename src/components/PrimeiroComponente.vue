<template>
    <div>
        <h1>Ola vue!</h1>
        <p>Meu nome é {{ nome }}</p>
        <p>Funcao: {{ profissao }}</p>
        <MultiplosEventos />
    </div>
</template>

<script>

import MultiplosEventos from './MultiplosEventos.vue'

export default {
    name: 'Primeiro componente',
    components: {
        MultiplosEventos
    },
    data() {
        return {
            nome: "Bruno",
            profissao: 'Programador'
        }
    }
}
</script>