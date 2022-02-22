<template>
    <div class="paragrafo-pai">
        <Picture />
        <h2>Essa é a descrição da Pessoa: {{ nome }} </h2>
        <Info />
        <Form />
    </div>
</template>

<script>

import Info from './Info.vue'
import Form from './Form.vue'
import Picture from './Picture.vue'



export default {
    name: 'Pessoa',
    components: {
        Info,
        Form,
        Picture
    },
    data () {
        return {
            nome: 'Bruno'
        }
    }, 
}
</script>