<template>
  <main>
    <ul>
      <li v-for="produto in $store.state.cart" :key="produto">
        <img :src="produto.image" :alt="produto.name">
        <h1>{{produto.name}} <span class="green">comprado</span></h1>
      </li>
    </ul>
  </main>
</template>
<script>
export default{
  name: 'Carrinho'
}
</script>

<style scoped>
  main{
    width: 100%;
  }
  main ul {
    list-style-type: none;
    width: 100%;
    max-width: 1280px;
    padding: 15px 2%;
    display: flex;
    gap: 15px;
    flex-wrap: wrap;
    justify-content: center;
  }

  .green{
    color: greenyellow;
  }
  main ul li{
    width: 100%;
    max-width: 300px;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
  li img{
    width: 100%;
  }
</style>