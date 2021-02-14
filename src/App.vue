<template>
  <div id="app">
    <Header />
    <NavbarTop />
    <CarouselComponent />
    <Content />
    <Footer />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import NavbarTop from "./components/NavbarTop.vue";
import CarouselComponent from "./components/Carousel.vue";
import Content from "./components/Content.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    NavbarTop,
    CarouselComponent,
    Content,
    Footer,
  },
};
</script>

<style lang="scss">
@import url(//db.onlinewebfonts.com/c/1ae0d8aae01cff8acccef4590bb4a51b?family=Neue+Helvetica);

#app {
  font-family: "Neue Helvetica W06", "Helvetica Neue", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
