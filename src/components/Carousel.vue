<template>
  <carousel :paginationPadding="5" :perPage="1">
    <slide style="justify-content: center">
      <div class="imgWrapper">
        <div class="row linkRow">
          <a href="/">
            <h2>Sinu <strong>hea tegu</strong></h2>
            <br />
            <a class="lookCloser">
              Vaata lähemalt<svg
                xmlns="http://www.w3.org/2000/svg"
                width="16"
                height="16"
                fill="currentColor"
                class="bi bi-arrow-right"
                viewBox="0 0 16 16"
                style="margin-left: 5px"
              >
                <path
                  fill-rule="evenodd"
                  d="M1 8a.5.5 0 0 1 .5-.5h11.793l-3.147-3.146a.5.5 0 0 1 .708-.708l4 4a.5.5 0 0 1 0 .708l-4 4a.5.5 0 0 1-.708-.708L13.293 8.5H1.5A.5.5 0 0 1 1 8z"
                /></svg
            ></a>
          </a>
        </div>
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
.linkRow {
  width: 1170px;
  display: block;
  margin-left: auto;
  margin-right: auto;
  z-index: 1;
  text-align: left;
  padding-left: 8%;
  h2 {
    color: #32344c;

    font-size: 62px;
    font-weight: 100;
    line-height: 62px;
  }
  strong {
    font-weight: 600;
  }
  a {
    cursor: pointer;

    color: black;
    text-decoration: none;
    font-weight: bold;
  }
}
.imgWrapper {
  height: 500px;
  overflow: hidden;
  position: relative;
  display: inline-flex;
  align-items: center;
  width: 100%;
}
.bgImg {
  height: 500px;
  position: absolute;
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