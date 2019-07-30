<template>
  <div class="separator">
    <div class="wrapper">
      <h2>#Yo voto</h2>
      <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Veniam enim dignissimos vero pariatur corporis odit cum consequuntur quas iste atque, minus sequi similique quos. Nihil assumenda qui voluptatum aspernatur eos.</p>
      <!-- <div class="columns is-desktop">
        <div class="column">
          <h3>Title</h3>
          <p class="description">Lorem ipsum dolor sit, amet consectetur adipisicing elit. Itaque, natus tempore distinctio voluptatem odio consequuntur rerum consectetur laborum fuga repellendus corrupti possimus ipsam nam</p>
        </div>
        <div class="column">
          <h3>Title</h3>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Itaque, natus tempore distinctio voluptatem odio consequuntur rerum consectetur laborum fuga repellendus corrupti possimus ipsam nam</p>
        </div>
        <div class="column">
          <h3>Title</h3>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Itaque, natus tempore distinctio voluptatem odio consequuntur rerum consectetur laborum fuga repellendus corrupti possimus ipsam nam</p>
        </div>
      </div> -->

    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.separator {
  width: 100%;
  background-color: rgba(77, 89, 97, 0.051);
}
.wrapper {
  max-width: 1344px;
  margin: 0px auto;
  padding: 40px 12px 60px;
}
/* h3 {
  font-weight: 600;
  color: #2a2f53;
}
p {
  padding: 10px 0 30px;
  color: #3d506d;
} */
h2 {
  text-align: center;
  font-weight: 600;
  font-size: 3rem;
  color: #4d5961;
  line-height: 1;
}
p {
  margin-top: 20px;
  text-align: center;
  color: #2a2f53;
  font-style: oblique;
  font-size: 18px;
}
@media (max-width: 1024px) {
  .wrapper {
    padding: 20px 12px;
  }
  h2 {
    font-size: 3rem;
  }
}
</style>
