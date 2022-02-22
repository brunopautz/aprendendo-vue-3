<template>
    <div>
        <p> {{ email }} </p>
        <p v-if="esta_trabalhando" >Estou trablhando no momento</p>
        <p v-else>Estou em busca de novas oportunidades</p>
        <p>Utilizo as seguintes tech para back end:</p>
        <ul> 
            <li v-for="(tech, index) in techs_back" v-bind:key="index">{{ tech }}</li>
        </ul>
        <p>Utilizo as seguintes tech para fornt</p>
        <ul>
            <li v-for="tech in techs_front" :key="tech.id"> {{ tech.language }} </li>
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
    props : {
        email : String,
        esta_trabalhando : Boolean
    },
    data() {
        return {
            mostra_email: false,
            meu_link: 'https://google.com',
            textoBotao: 'Mostrar email',
            techs_back: ['PHP', 'PYTHON', 'C', 'Java'],
            techs_front: [
                {id: 1, language: "Html"},
                {id: 1, language: "Vue"},
                {id: 1, language: "React"}
            ],

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

<style>
    .paragrafo-pai {
        background-color: black;
    }
</style>