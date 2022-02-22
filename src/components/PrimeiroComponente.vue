<template>
    <div>
        <h1>Ola vue!</h1>
        <Reutilizando />

        <p>Meu nome é {{ nome }}</p>
        <p>Funcao: {{ profissao }}</p>
        <MultiplosEventos />
        <Reutilizando />
        <Reutilizando />
        <Reutilizando />
        <Reutilizando />
        <Reutilizando />

    </div>
</template>

<script>

import MultiplosEventos from './MultiplosEventos.vue'
import Reutilizando from './Reutilizando.vue'

export default {
    name: 'Primeiro componente',
    components: {
        MultiplosEventos,
        Reutilizando
    },
    data() {
        return {
            nome: "Bruno",
            profissao: 'Programador'
        }
    }
}
</script>