<template>
  <div class="theme container-page">
    <nav class="navbar ">
      <div class="container">
        <div class="navbar-brand">
          <nuxt-link
            class="logo"
            to="/"
          >
            <h1 class="logo-name-two">Alexander Quevedo</h1>
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
              @click.native="toggleItem(index)"
            >{{item.name}}</nuxt-link>
            <div class="navbar-item wrapper-icons-nav">
              <a
                href="https://www.facebook.com/Alexander-Quevedo-349850775734108/"
                class="link"
                target="_blank"
              >
                <i class="icon-facebook"></i>
              </a>
              <a
                href="#"
                class="link"
              >
                <i class="icon-twitter"></i>
              </a>
              <a
                href="#"
                class="link"
              >
                <i class="icon-youtube-play"></i>
              </a>
            </div>
          </div>
        </div>
      </div>
    </nav>
    <nuxt />
    <Footer />
  </div>
</template>

<script>
import Footer from "../components/Footer";
export default {
  components: {
    Footer
  },
  data() {
    return {
      nav: [
        {
          path: "/",
          name: "Inicio"
        },
        {
          path: "MyStory",
          name: "Quién Soy?"
        },
        {
          path: "OurCity",
          name: "Plan de Gobierno"
        },
        {
          path: "OurCity",
          name: "Gestión en la Asamblea"
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
      this.$refs.burger.classList.toggle("is-active");
      this.$refs.toggleMenu.classList.toggle("is-active");
    }
  }
};
</script>

<style>
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
  /* padding: 8px 12px; */
  color: #4a4a4a !important;
  font-weight: 600;
  font-size: 1.5rem;
}
.logo {
  display: flex;
  align-items: center;
  margin-left: 12px;
}
.wrapper-icons-nav {
  width: 100px;
  display: flex;
  justify-content: space-between;
}
.wrapper-icons-nav > a {
  color: #4a4a4a;
}
.wrapper-icons-nav > a:hover {
  color: var(--orange);
}
@media (max-width: 800px) {
  .logo-name-two {
    font-size: 1rem;
    /* padding: 7px 12px; */
  }
}
</style>
