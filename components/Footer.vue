<template>
  <div class="footer">
    <div class="logo">
      <span>Alexander</span>
      <span>Quevedo</span>
    </div>
    <div class="bottom">
      <p class="copy">&copy; copyright 2019 - Hecho con <i class="heart icon-heart"></i> por sublimax.com</p>
      <div class="wrapper-icons">
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
</template>

<script>
export default {};
</script>

<style scoped>
.footer {
  width: 100%;
  background: #333;
  color: rgba(255, 255, 255, 0.815);
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  position: relative;
  padding-top: 1.2rem;
}
.logo {
  display: flex;
  flex-direction: column;
  line-height: 1;
}
.logo > span:nth-child(1) {
  font-size: 1.1rem;
  position: relative;
  top: 8px;
  letter-spacing: 1px;
}
.logo > span:nth-child(2) {
  font-size: 2rem;
  font-weight: 600;
}
.bottom {
  width: 100vw;
  position: absolute;
  bottom: 0;
  left: 0;
  background-color: rgba(0, 0, 0, 0.4);
  display: flex;
  justify-content: space-between;
  box-sizing: border-box;
  padding: 10px 40px;
  align-items: center;
}
.bottom a {
  color: rgba(255, 255, 255, 0.815);
  border: 2px solid rgba(255, 255, 255, 0.815);
  width: 30px;
  height: 30px;
  border-radius: 50%;
  display: flex;
  justify-content: center;
  align-items: center;
  margin: 0 7px;
}
.bottom a i {
  line-height: 1;
  position: relative;
  top: 1px;
  font-size: 14px;
}
.bottom a:hover {
  color: var(--orange);
  border: 2px solid var(--orange);
}
.wrapper-icons {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100%;
  padding: 10px;
  /* min-height: 40px; */
}
.copy {
  font-weight: 300;
  opacity: 0.2;
  line-height: 1;
  vertical-align: middle;
}
.heart {
  font-size: 10px;
}
@media (max-width: 1024px) {
  .bottom {
    flex-direction: column-reverse;
    text-align: center;
  }
  .copy {
    padding-top: 10px;
  }
  .footer {
    min-height: 220px;
  }
}
</style>
