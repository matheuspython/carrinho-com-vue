<template>
  <div>
    <img :src="image" :alt="name" />
    <h1>{{ name }}</h1>
    <p>{{ description }}</p>
    <button @click="addToCart">comprar {{ price }}R$</button>
  </div>
</template>

<script>
export default {
  name: "Product",
  props: {
    image: String,
    name: String,
    description: String,
    price: Number,
  },
  methods: {
    addToCart() {
      this.$store.commit("addProduct", {
        image: this.image,
        name: this.name,
        description: this.description,
        price: this.price,
      });
    },
  },
};
</script>

<style scoped>
div {
  border-radius: 12px;
  width: 100%;
  max-width: 300px;
  background: #632b74;
  display: flex;
  flex-direction: column;
  align-items: center;
  padding: 15px;
  gap: 15px;
}
div img {
  width: 100%;
  border-radius: 12px 12px 0 0;
}

div button {
  width: 80%;
  max-width: 300px;
  border: 1px solid white;
  height: 35px;
  color: #fff;
  border-radius: 12px;
  background: transparent;
  transition: 0.4s;
  cursor: pointer;
}
div button:hover {
  background: #fff;
  color: #632b74;
}
</style>
