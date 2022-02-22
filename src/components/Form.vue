<template>
   <div>
       <h2>Meu formulario: </h2>
        <form action="" @submit="enviarFormulario($event)">
            <div>
               <input type="text" v-model="name">
            </div>
            <div>
               <input type="text" v-model="email">
            </div>
            <Submit />
        </form>
   </div>
</template>

<script>

import InputText from './form/InputText.vue'
import Submit from './form/Submit.vue'

export default {
    name: 'Form',
    components: {
        InputText,
        Submit
    }, 
    data() {
       return {
            name: '',
            email: ''
       }
    },
    methods: {
        enviarFormulario (e) {

            const name = this.name
            const email = this.email
            
            e.preventDefault();
            console.log('formulario enviado');

            console.log('Name: ' + name);
            console.log('Email: ' + email);

        }
    }
}
</script>