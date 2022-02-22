<template>
    <div>
        <button @click="$emit('mudarImagem')" >Mudar imagem perfil</button>
    </div>
</template>

<script>
export default {
    name: 'MudarImg',
    emits: ['mudarImagem']
}
</script>