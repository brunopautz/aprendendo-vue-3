<template>
    <div>
        <ul>
            <li><a href="">Home</a></li>
            <li><a href="">Projeto</a></li>
            <li><a href="">Sobre</a></li>
            <li><a href="">Contato</a></li>
            <li v-show="esta_logado"><a href="">Meu perfil</a></li>
        </ul>
    </div>
</template>

<script>
export default {
    name: 'Header',
    props: ['esta_logado']
}
</script>

<style scoped>
    ul {
        list-style: none;
        display: flex;
        background-color: #999;
    }

    li {
        margin-right: 10px;
    }

    a {
        color: #ddd;
        text-decoration: none;
        transition: .5s;
    }

    a:hover {
        color: turquoise;
    }
</style>