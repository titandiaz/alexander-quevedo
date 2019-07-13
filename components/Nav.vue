<template>
  <section class="hero bg-banner is-large">
    <!-- Hero head: will stick at the top -->
    <div class="hero-head">
      <header class="navbar">
        <div class="container">
          <div class="navbar-brand">
            <a class="">
              <h1 class="title logo-name">Alexander Quevedo</h1>
            </a>
            <span
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
          >
            <div class="navbar-end">
              <a class="navbar-item is-active">
                Home
              </a>
              <a class="navbar-item">
                Examples
              </a>
              <a class="navbar-item">
                Documentation
              </a>
            </div>
          </div>
        </div>
      </header>
    </div>

    <!-- Hero content: will be in the middle -->
    <div class="hero-body">
      <div class="container has-text-centered">
        <h1 class="title">
          Title
        </h1>
        <h2 class="subtitle">
          Subtitle
        </h2>
      </div>
    </div>
  </section>
</template>

<script>
export default {};
</script>

<style>
.logo-name {
  padding: 8px 12px;
}
.bg-banner {
  background-color: var(--verde);
}
</style>
