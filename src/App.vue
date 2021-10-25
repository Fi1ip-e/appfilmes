<template>
  <div id="app">
    <Jumb />
    <div>
    <Menu />
      <Carousel />
      <Home />
      
    </div>
  </div>
</template>

<script>
import Jumb from "./components/Jumb.vue";
import Menu from "./components/Menu.vue";
import Carousel from "./components/Carousel.vue";
import Home from "./components/Home.vue";
export default {
  name: "App",
  components: {
    Jumb,
    Menu,
    Carousel,
    Home,
    
  },
};
</script>

<style>
body {
  margin: 0;
  background: #FFFFE0 !important;
  font-family: "Playfair Display", serif !important;
}
.container {
  background: white;
  margin-top: 1.5rem;
  margin-bottom: 1rem;
  padding-bottom: 1rem;

  
  box-shadow: 0 1px 4px 3px rgb(73, 73, 73);
  /* background-image: linear-gradient(#031625, #112e46, #031625, #112e46, #031625); */
}
</style>
