<template>
  <div class="container-page">
    <!-- <Nav /> -->
    <Swiper />
    <div class="line"></div>
    <Separator />
    <Features />
  </div>
</template>

<script>
// import Nav from "~/components/Nav";
import YoVoto from "~/components/YoVoto";
import Swiper from "~/components/Banner";
import Separator from "~/components/Separator";
import Features from "~/components/Features";
export default {
  layout: "secondary",
  pageTransition: "OurCity",
  components: {
    // Nav,
    YoVoto,
    Swiper,
    Separator,
    Features
  },
  data() {
    return {};
  }
};
</script>

<style scoped>
.line {
  width: 100%;
  height: 10px;
  background: linear-gradient(
    to right,
    rgb(255, 59, 25) -17%,
    rgba(255, 180, 51, 1) 50%,
    rgba(0, 168, 0, 1) 98%
  );
}
@media (max-width: 800px) {
  .line {
    height: 5px;
  }
}
</style>
