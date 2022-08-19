<template>
  <TheHeader />
  <router-view/>
</template>
<script>
import TheHeader from './components/TheHeader.vue';
export default {
    components: { TheHeader }
}
</script>
<style>
*{
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}
html, body{
  /* font-family: 'Roboto', sans-serif; */
  font-family: 'Manrope', sans-serif;
}
body{
  background: #202020;
  color: #fff;
}
a{
  text-decoration: none;
}
ul{
  list-style-type: none;
}
</style>
