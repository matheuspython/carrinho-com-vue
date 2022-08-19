<template>
  <section>
    <Product v-for="produto in $store.state.products" :key="produto" :image="produto.image" :name="produto.name" :price="produto.price" :description="produto.description" />

  </section>
</template>

<script>
import Product from './ProductVue.vue';
export default {
    components: { Product }
}
</script>

<style scoped>
  section{
    width: 100%;
  display: flex;
  justify-content: center;
  align-items: center;
  gap: 15px;
  
  flex-wrap: wrap;
}
</style>