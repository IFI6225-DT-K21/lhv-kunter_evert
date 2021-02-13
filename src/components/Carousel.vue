<template>
  <carousel :paginationPadding="5" :perPage="1">
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
      <div class="imgWrapper">
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
      </div>
    </slide>
    <slide>
      <div class="imgWrapper">
        <img
          class="bgImg"
          src="https://www.lhv.ee/assets/images/headers/palkyle-bg.svg"
          alt="First slide"
        />
        <img
          class="fgImg"
          src="https://www.lhv.ee/assets/images/headers/palkyle-fg.svg"
          alt="First slide"
        />
      </div>
    </slide>
    <slide>
      <div class="imgWrapper">
        <img
          class="bgImg"
          src="https://www.lhv.ee/assets/images/headers/pension-2021-bg.svg"
          alt="First slide"
        />
        <img
          class="fgImg"
          src="https://www.lhv.ee/assets/images/headers/pension-2021-fg.svg"
          alt="First slide"
        />
      </div>
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
.VueCarousel-dot-container {
  margin-top: 0 !important;
}
.imgWrapper {
  height: 500px;
  overflow: hidden;
  position: relative;
  display: inline-flex;

  width: 100%;
}
.bgImg {
  height: 500px;
  width: 100%;
  -webkit-background-size: cover;
  -moz-background-size: cover;
  -o-background-size: cover;
  background-size: cover;
  object-fit: cover;
}
.fgImg {
  position: absolute;
  height: 550px;
  min-width: 100%;
}
.carousel-indicators li {
  background-color: black;
}
</style>