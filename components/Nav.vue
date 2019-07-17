<template>
  <section class="hero bg-banner is-large bg-img">
    <!-- Hero head: will stick at the top -->
    <div class="hero-head">
      <header class="navbar title-header">
        <div class="container">
          <div class="navbar-brand">
            <nuxt-link
              to="/"
              class="logo-name"
            >
              <h1 class="title logo-name">Alexander Quevedo</h1>
            </nuxt-link>
            <span
              ref="burger"
              @click="toggle"
              class="navbar-burger burger"
              data-target="navbarMenuHeroC"
            >
              <span></span>
              <span></span>
              <span></span>
            </span>
          </div>
          <div
            id="navbarMenuHeroC"
            class="navbar-menu"
            ref="toggleMenu"
          >
            <div class="navbar-end">
              <nuxt-link
                to="/"
                class="navbar-item is-active"
              >
                Inicio
              </nuxt-link>
              <nuxt-link
                class="navbar-item"
                to="/MyStory"
              >Mi Historia</nuxt-link>
              <nuxt-link
                class="navbar-item"
                to="/OurCity"
              >Nuestra Ciudad</nuxt-link>
            </div>
          </div>
        </div>
      </header>
    </div>

    <!-- Hero content: will be in the middle -->
    <div class="wrapper-slider">
      <Swiper />
    </div>
  </section>
</template>

<script>
import Swiper from "~/components/Banner";
export default {
  components: {
    Swiper
  },
  methods: {
    toggle() {
      this.$refs.burger.classList.toggle("is-active");
      this.$refs.toggleMenu.classList.toggle("is-active");
    }
  }
};
</script>

<style>
.logo-name {
  padding: 8px 12px;
  color: #ffffff;
}
.bg-banner {
  background-color: var(--orange);
}
.bg-img {
  background-image: url("../assets/img/personas2.jpg");
  background-repeat: no-repeat, repeat;
  background-position-y: 0%;
  background-size: cover;
}
.wrapper-slider {
  z-index: 0;
}
</style>
