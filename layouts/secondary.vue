<template>
  <div class="theme container-page">
    <nav class="navbar ">
      <div class="container">
        <div class="navbar-brand">
          <nuxt-link
            to="/"
            class="logo-name-two"
          >
            <h1 class="title logo-name-two">Alexander Quevedo</h1>
          </nuxt-link>
          <span
            @click="toggle"
            ref="burger"
            class="navbar-burger burger"
            data-target="navMenu"
          >
            <span></span>
            <span></span>
            <span></span>
          </span>
        </div>
        <div
          class="navbar-menu"
          ref="toggleMenu"
        >
          <div class="navbar-end">
            <nuxt-link
              v-for="(item, index) in nav"
              :key="index"
              :to="item.path"
              class="navbar-item"
              :class="selected === index ? 'is-active' : ''"
              @click="toggleItem(index)"
            >{{item.name}}</nuxt-link>
          </div>
        </div>
      </div>
    </nav>
    <nuxt />
  </div>
</template>

<script>
export default {
  data() {
    return {
      nav: [
        {
          path: "/",
          name: "Inicio"
        },
        {
          path: "MyStory",
          name: "Mi Historia"
        },
        {
          path: "OurCity",
          name: "Nuestra Ciudad"
        }
      ],
      selected: 0
    };
  },
  methods: {
    toggle() {
      this.$refs.burger.classList.toggle("is-active");
      this.$refs.toggleMenu.classList.toggle("is-active");
    },
    toggleItem(index) {
      this.selected = index;
    }
  }
};
</script>

<style>
:root {
  --orange: #f87218;
  --yellow: #f7b733;
  --green: #4abdac;
}
* {
  font-family: "Montserrat", sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
.logo-name-two {
  padding: 8px 12px;
  color: #4a4a4a !important;
}
</style>
