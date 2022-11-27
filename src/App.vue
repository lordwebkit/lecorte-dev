<script setup>
import Header from "./components/Header.vue"
import Preview from "./components/Preview.vue";
import Introduction from "./components/Introduction.vue";
import Collection from "./components/Collection.vue";
import Tasting from "./components/Tasting.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
  <div class="header-wrapper header-wrapper_preview-bg">
    <div class="grid-wrapper">
      <Header></Header>
    </div>
    <div class="grid-wrapper">
      <Preview />
    </div>
  </div>

  <div class="introduction-wrapper black_bg">
    <div class="grid-wrapper">
      <Introduction />
    </div>
  </div>

  <!-- <div class="collection-wrapper beige_bg">
    <div class="grid-wrapper">
      <Collection />
    </div>
  </div>

  <div class="tasting-wrapper black_bg">
    <div class="grid-wrapper">
      <Tasting />
    </div>
  </div>

  <div class="footer-wrapper">
    <div class="grid-wrapper">
      <Footer></Footer>
    </div>
  </div> -->
</template>

<style scoped>
.header-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  padding-bottom: 150px;
}
.header-wrapper_preview-bg {
    width: 100%;
    height: 100vh;
    background-image: url("./assets/preview-bg.png");
    background-size: cover;
}

.introduction-wrapper {
  padding-top: 100px;
  padding-bottom: 100px;
}

.collection-wrapper {
  padding: 80px 0;
}

.footer-wrapper {
  background-color: #998431;
  padding: 50px 0;
}

.tasting-wrapper {
  padding: 100px 0;
}

.black_bg {
  background-color: #282828;
}

.beige_bg {
  background-color: #E6E3C4;
}
</style>
