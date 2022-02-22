<template>
    <div>
        <p v-if="esta_trabalhando" >Estou trablhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tec:</p>
        <ul>
            <li>Javascript</li>
            <li>PHP</li>
            <li>Python</li>
        </ul>
        <div>
            <button @click="showEmail"> {{ textoBotao }} </button>
        </div>
        <p v-show="mostra_email">Contato: {{ email }}</p>
        <p>Para acessar meu portifolio <a v-bind:href="meu_link">basta clicar aqui</a></p>
    </div>
</template>

<script>
export default {
    name: 'Info',
    data() {
        return {
            esta_trabalhando: false,
            mostra_email: false,
            email: 'brunoppaytz@gmail.com',
            meu_link: 'https://google.com',
            textoBotao: 'Mostrar email'
        }
    },
    methods: {
        showEmail() {
            this.mostra_email = !this.mostra_email

            if (this.mostra_email) {
                this.textoBotao = 'Esconder email'
            } else {
                this.textoBotao = 'Mostrar email'
            }
        }
    }
}
</script>