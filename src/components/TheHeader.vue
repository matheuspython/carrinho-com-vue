<template>
  <header>
    <nav>
        <router-link to="/">loja</router-link> |
        <router-link to="/carrinho">carrinho</router-link>
    </nav>
  </header>
</template>

<script>
export default {
    name: 'TheHeader'
}
</script>

<style scoped>
    header{
        width: 100%;
        height: 65px;
        background: #760cf0;
}
header nav {
    width: 100%;
    height: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 15px;
    color: #fff;
}
header a {
    color: #fff;
}
</style>