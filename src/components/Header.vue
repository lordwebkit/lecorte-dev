<script setup>
import NavBar from "./NavBar.vue"
</script>
<template>
  <div class="header-wrapper wrapper">
    <header class="header">
      <div class="header-info">
        <div class="header-info__link-wrapper header-info__link-adress-wrapper">
          <a target="_blank"
            href="https://yandex.ru/maps/213/moscow/house/prospekt_vernadskogo_41/Z04YcwdjTUMPQFtvfXp2dXlqZA==/?ll=37.503469%2C55.674590&z=17.09"
            class="header-info__link header-info-adress">проспект Вернадского, 41</a>
        </div>
        <div class="header-info__link-wrapper header-info__link-phone-wrapper">
          <a href="./" class="header-info__link header-info-phone">8 (812) 123-45-67</a>
        </div>
        <div class="header-info__burger header-burger">
          <span class="header-burger__line"></span>
        </div>
      </div>
      <NavBar />
    </header>
  </div>
</template>


<style scoped>
.header-info {
  display: flex;
  justify-content: space-between;
  margin-bottom: 20px;
  padding-top: 10px;
}

.header-info__link {
  color: #fff;
  text-decoration: none;
  font-size: 13px;
  line-height: 150%;
}

.header-info__burger {
  display: none;
}

@media screen and (max-width: 670px) {
  .header-info__burger {
    display: flex;
    justify-content: space-between;
    flex-direction: column;
  }

  .header-burger__line {
    display: inline-block;
    width: 40px;
    height: 2px;
    background-color: #fff;
  }

  .header-info__burger::before,
  .header-info__burger::after {
    content: "";
    width: 40px;
    height: 2px;
    display: block;
    background-color: #fff;
  }

  .header-info__link {
    font-size: 15px;
  }
}

@media screen and (max-width: 560px) {
  .header-info__link-phone-wrapper {
    display: none;
  }
}
</style>