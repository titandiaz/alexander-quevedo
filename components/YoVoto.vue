<template>
  <div class="columns is-mobile yo-voto">
    <div class="column is-half is-4 box-voto">
      <h2 class="title-yo-voto">#Yo voto</h2>
      <div class="more">mas información</div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.box-voto {
  margin: 0 auto;
  padding: 0.5rem 3rem;
  border-radius: 20px;
  background-color: var(--green);
  position: relative;
  /* top: -3rem; */
  z-index: 99;
}
.title-yo-voto {
  font-weight: bold;
  color: #fff;
  font-size: 3.8rem;
}
.more {
  background: linear-gradient(
    to right,
    rgb(255, 59, 25) -17%,
    rgba(255, 180, 51, 1) 50%,
    rgba(0, 168, 0, 1) 98%
  );
  color: #fff;
  display: inline-block;
  padding: 0.5rem 1rem;
  border-radius: 8px;
  font-weight: bold;
  position: absolute;
  bottom: -1rem;
  right: 55%;
  cursor: pointer;
}
</style>
