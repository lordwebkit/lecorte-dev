<script setup>
</script>
<template>
    <footer id="footer" class="footer">
        <nav class="nav-bar">
            <div class="nav-bar-menu nav-bar__menu">
                <a href="./" class="nav-bar__button-wrapper">
                    <p class="nav-bar__button">Главная</p>
                </a>
                <a href="./" class="nav-bar__button-wrapper">
                    <p href="./" class="nav-bar__button">Каталог</p>
                </a>
                <a href="./" class="nav-bar__button-wrapper">
                    <p href="./" class="nav-bar__button">Поставщики</p>
                </a>
                <a href="./" class="nav-bar__button-wrapper">
                    <p href="./" class="nav-bar__button">Коллекции</p>
                </a>
                <a href="./" class="nav-bar__button-wrapper">
                    <p href="./" class="nav-bar__button">Дегустация</p>
                </a>
                <a href="./" class="nav-bar__button-wrapper">
                    <p href="./" class="nav-bar__button">Коллекция 2022</p>
                </a>
                <a href="./" class="nav-bar__button-wrapper">
                    <p href="./" class="nav-bar__button">Контакты</p>
                </a>
            </div>
            <div class="nav-bar-contact nav-bar__contact">
                <a href="./" class="nav-bar-contact__button-wrapper nav-bar__button-wrapper">
                    <p class="nav-bar-contact__button nav-bar__button">винный бутик LE CORTE</p>
                </a>
                <a href="./" class="nav-bar-contact__button-wrapper nav-bar__button-wrapper">
                    <p href="./" class="nav-bar-contact__button nav-bar__button">8 (812) 123-45-67</p>
                </a>
                <a href="./" class="nav-bar-contact__button-wrapper nav-bar__button-wrapper">
                    <p href="./" class="nav-bar-contact__button nav-bar__button nav-bar-social">
                        <span class="nav-bar-contact__button-social nav-bar-social__youtube"></span>
                        <span class="nav-bar-contact__button-social nav-bar-social__vk"></span>
                        <span class="nav-bar-contact__button-social nav-bar-social__fb"></span>
                    </p>
                </a>
                <a href="./" class="nav-bar-contact__button-wrapper nav-bar__button-wrapper">
                    <p href="./" class="nav-bar-contact__button nav-bar__button">© le-corte.ru</p>
                </a>
            </div>
        </nav>
    </footer>
</template>


<style scoped>
.nav-bar-menu,
.nav-bar-contact {
    display: flex;
    height: 60px;
    border-bottom: 1px solid #fff;
}

.nav-bar-menu {
    border-top: 1px solid #fff;

}

.nav-bar-contact {
    text-transform: uppercase;
}

.nav-bar__button {
    color: #fff;
    text-align: center;
    flex: 1;
    font-size: 14px;
    line-height: 150%;
}

.nav-bar-contact__button {
    font-weight: 700;
}

.nav-bar-social {
    display: flex;
    justify-content: space-around;
    align-items: center;
    padding: 0 23px;
}

.nav-bar-social__youtube {
    width: 23px;
    height: 16px;
    background-image: url("../assets/youtube-icon.svg");
}

.nav-bar-social__vk {
    width: 24px;
    height: 14px;
    background-image: url("../assets/vk-icon.svg");
}

.nav-bar-social__fb {
    width: 11px;
    height: 20px;
    background-image: url("../assets/fb-icon.svg");
}


.nav-bar__button-wrapper {
    flex: 1;
    align-items: center;
    display: flex;
    text-decoration: none;
}

.nav-bar-contact__button-wrapper {
    border-right: solid #fff 1px;
}

.nav-bar-contact__button-wrapper:last-child {
    border-right: none;
}

.nav-bar__button-wrapper:hover {
    background-color: rgba(255, 255, 255, 0.089);
}

.nav-bar__button-wrapper:active {
    background-color: rgba(0, 0, 0, 0.123);
}
</style>