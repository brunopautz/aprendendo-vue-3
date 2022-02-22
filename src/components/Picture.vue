<template>
    <div>
        <img :src="avatar" :alt="descricao">
        <MudarImg  @mudar-imagem="trocarImagem" />
    </div>
</template>

<script>

import MudarImg from './MudarImg.vue'

export default {
    name: 'Picture',
    components: {
        MudarImg
    },
    data () {
        return {
            avatar: '/image/avatar.png',
            descricao: 'Bruno Pautz'
        }
    },
    methods: {
        trocarImagem(){
            this.avatar = '/image/avatar2.png'
        }
    }
}
</script>