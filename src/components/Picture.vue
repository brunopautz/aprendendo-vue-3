<template>
    <div>
        <img :src="avatar" :alt="descricao">
    </div>
</template>

<script>
export default {
    name: 'Picture',
    data () {
        return {
            avatar: '/image/avatar.png',
            descricao: 'Bruno Pautz'
        }
    }
}
</script>