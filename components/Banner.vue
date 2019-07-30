<template>
  <div v-swiper:mySwiper="swiperOption">
    <div class="swiper-wrapper">
      <div class="center">
        <img src="../assets/img/banner.jpeg">
      </div>
    </div>
    <div class="swiper-pagination swiper-pagination-bullets"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      swiperOption: {
        loop: true,
        slidesPerView: "auto",
        centeredSlides: true,
        spaceBetween: 30,
        pagination: {
          el: ".swiper-pagination",
          dynamicBullets: true
        }
      }
    };
  }
};
</script>

<style scoped>
.center {
  width: 100vw;
  display: flex;
  justify-content: center;
}
.center img {
  width: 100%;
  object-fit: cover;
}
</style>
