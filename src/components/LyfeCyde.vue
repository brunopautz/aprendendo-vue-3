<template>
    <h1>Meu nome é: {{ nome }} </h1>
</template>

<script>
export default {
    name: 'LyfeCyde',
    data() {
        return {
            nome: 'Ainda nao sei'
        }
    },
    created() {
        setTimeout(() => {
            this.nome = 'Bruno'
        }, 1000)
    },
    mounted() {
         setTimeout(() => {
            this.nome = 'Joao'
        }, 2000)
    }
}
</script>