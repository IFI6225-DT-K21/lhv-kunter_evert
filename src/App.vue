<template>
  <div id="app">
    <Header />
    <NavbarTop />
    <CarouselComponent />
    <Content />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import NavbarTop from "./components/NavbarTop.vue";
import CarouselComponent from "./components/Carousel.vue";
import Content from "./components/Content.vue";

export default {
  name: "App",
  components: {
    Header,
    NavbarTop,
    CarouselComponent,
    Content,
  },
};
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
