<template>
  <div class="separator">
    <div class="wrapper">
      <!-- <h2>Presentación</h2> -->
      <p>Quiero lograr un municipio desarrollado, con oportunidades, que preserve el medio ambiente y mejore la calidad de vida de sus habitantes. Mi vida da fe de un compromiso social que me permite ser garantía de un cambio a la hora de gobernar, donde no cabe oportunidad a la corrupción, a la improvisación o al desorden administrativo; la eficiencia en los procesos, gestión y articulación interinstitucional serán pilares de nuestra administración municipal</p>
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
