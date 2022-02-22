<template>
    <div>
        <h1>Ola vue!</h1>
        <p>Meu nome é {{ nome }}</p>
        <p>Funcao: {{ profissao }}</p>

    </div>
</template>

<script>
export default {
    name: 'Primeiro componente',
    data() {
        return {
            nome: "Bruno",
            profissao: 'Programador'
        }
    }
}
</script>