<template>
  <carousel :perPage="1">
    <slide>
      <div class="imgWrapper">
        <img
          class="bgImg"
          src="https://www.lhv.ee/assets/images/headers/heategu-bg.svg"
          alt="First slide"
        />
        <img
          class="fgImg"
          src="https://www.lhv.ee/assets/images/headers/heategu-fg.svg"
          alt="First slide"
        />
      </div>
    </slide>
    <slide>
      <img
        class="bgImg"
        src="https://www.lhv.ee/assets/images/headers/parimpank-2021-bg.svg"
        alt="First slide"
      />
      <img
        class="fgImg"
        src="https://www.lhv.ee/assets/images/headers/parimpank-2021-fg.svg"
        alt="First slide"
      />
    </slide>
  </carousel>
</template>

<script>
// import $ from "jquery";
import { Carousel, Slide } from "vue-carousel";

export default {
  name: "CarouselComponent",
  components: {
    Carousel,
    Slide,
  },

  data() {
    return {};
  },
  mounted() {},
};
</script>

<style lang="scss" scoped>
.imgWrapper {
  height: 500px;
  overflow: hidden;
  z-index: 1000;
}
.bgImg {
  position: absolute;
  left: 0;
  right: 0;
  //   //   top: -56px;
  //   height: 600px;
  //   width: 100vw;
  //   background-position: center center;
  //   z-index: -100;
  z-index: -60;
  height: 500px;
}
.fgImg {
  left: 0;
  right: 0;
  width: 100%;
  z-index: -50;
  height: 600px;
}
.carousel-indicators li {
  background-color: black;
}
</style>