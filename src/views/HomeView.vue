<template>
  <main>
    <div class="container">
      <ProductList class="boxlist" />
    </div>
</main>
</template>

<script>
import ProductList from '@/components/products/ProductList.vue';
export default {
  name: 'HomeView',
  components: {
    ProductList
}
}
</script>
<style scoped>
  main {
    width: 100%;
  }
  main .container{
    width: 100%;
    max-width: 1280px;
    padding: 15px 2%;
  }
  .boxlist{
    width: 100%;
  }
</style>