<template>
  <div class="features">
    <div class="title title-features">Nuevo Titulo</div>
    <div class="grid">
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Otro Titulo</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Otro Titulo</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Otro Titulo</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Otro Titulo</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Otro Titulo</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
      <div class="feature">
        <div class="icon-description">
          <i class="icon-instagrem"></i>
        </div>
        <div class="description">
          <div class="title-description">Otro Titulo</div>
          <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Dicta eaque esse odit voluptas. Illo, officiis repellendus, cumque exercitationem amet ea, omnis.</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
.features {
  width: 100%;
  padding: 40px 10px;
  box-sizing: border-box;
}
.grid {
  margin: 0 auto;
  max-width: 1344px;
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(340px, 5fr));
  grid-gap: 40px;
}
.title-features {
  text-align: center;
  margin-bottom: 50px;
}
.feature {
  display: flex;
}
.icon-description {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: var(--orange);
  color: #fff;
  margin: 5px 10px 0 0;
}
.icon-description i {
  line-height: 1;
}
.description {
  flex: 1;
}
.description > p {
  color: #2a2f53;
}
.title-description {
  font-weight: 600;
  margin: 0 0 5px 0;
  color: #2a2f53;
}
@media (max-width: 1024px) {
  .grid {
    grid-template-columns: repeat(auto-fill, minmax(250px, 5fr));
  }
  .description > p {
    font-size: 14px;
  }
}
</style>
