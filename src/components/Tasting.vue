<template>
    <div id="tasting" class="tasting">
        <div class="tasting__header-wrapper">
            <div class="tasting__header-before header-before">
                <div class="header-before__el header-decore-el"></div>
            </div>
            <h2 class="tasting__header title_resize">Запись на дегустацию</h2>
            <div class="tasting__header-after header-after">
                <div class="header-after__el header-decore-el"></div>
            </div>
        </div>
        <div class="content-wrapper">
            <p class="tasting__text text_resize">
                В нашей коллекции собраны лучшие Вина Бордо.
                Прикоснитесь к искуству винного дела на нашей дегустации.
                Для этого отправьте заявку и дождитесь ответа нашей компании
            </p>
        </div>

        <form class="tasting-form tasting__form" action="" method="post">
            <div class="content-wrapper">
                <fieldset class="tasting-form__fieldset tasting-form__client-info">
                    <input class="tasting-form__field-name tasting-form__field" type="name" name="name"
                        placeholder="Имя">
                    <input class="tasting-form__field-phone tasting-form__field" type="phone" name="phone"
                        placeholder="Телефон">
                </fieldset>
                <fieldset class="tasting-form__fieldset tasting-form__location-info">
                    <input class="tasting-form__field-location tasting-form__field" type="text" name="location"
                        value="Бутик на Невском 103">
                </fieldset>
                <fieldset class="tasting-form__fieldset tasting-form__send-info">
                    <input class="tasting-form__button" type="button" name="register" value="Записаться">
                </fieldset>
            </div>
        </form>
    </div>
</template>

<style scoped>
.tasting {
    position: relative;
    color: #fff;
}

.tasting__form {
    padding: 80px 0;
    border: 3px solid #fff;
    border-top: none;
}

.tasting::before,
.tasting::after {
    content: "";
    background-color: #fff;
    display: inline-block;
    position: absolute;
}

.tasting::before {
    width: 260px;
    height: 260px;
    top: -40px;
    background-image: url("../assets/tasting-decore-grape.png");
}


.tasting::after {
    background-image: url("../assets/tasting-decore-barrel.png");
    width: 260px;
    height: 200px;
    right: -55px;
    top: -40px;
}

.content-wrapper {
    width: 540px;
    margin: 0 auto;
}

.tasting__header {
    text-align: center;
}

.tasting__header-wrapper {
    display: flex;
    align-items: flex-end;
    justify-content: center;
}

.header-after,
.header-before {
    flex: 1;
}

.header-before {
    text-align: right;
}

.tasting__header-before {
    margin-right: 35px;
}

.tasting__header-after {
    margin-left: 35px;
}

.header-decore-el {
    width: 75px;
    height: 3px;
    background-color: #fff;
    display: inline-block;
    margin-top: 0;
    margin-bottom: 20px;
    z-index: 2;
    flex: 1;
}

.header-after__el {
    width: 120px;
}

.tasting__text {
    line-height: 24px;
    text-align: center;
    font-weight: lighter;
}

.tasting__text::before {
    content: "";
    display: block;
    width: 118px;
    height: 1px;
    background-color: #fff;
    margin: 40px auto;
}

.tasting-form::after {
    content: "";
    width: 3px;
    height: 100px;
    background-color: #fff;
    display: block;
    position: absolute;
    right: -3px;
    top: -100px;
}

.tasting-form__fieldset {
    padding: 0;
    border: none;
}

.tasting-form__client-info {
    display: flex;
    justify-content: space-between;
}

.tasting-form__location-info {
    display: flex;
    margin-top: 40px;
    margin-bottom: 40px;
}

.tasting-form__send-info {
    display: flex;
    justify-content: center;
}

.tasting-form__field {
    background-color: transparent;
    border: none;
    border-bottom: 1px solid #fff;
    color: #fff;
    padding-bottom: 10px;
    font-size: 13px;
    font-family: 'Montserrat';
}

.tasting-form__field-name,
.tasting-form__field-phone {
    flex: 1;
}

.tasting-form__field-name {
    margin-right: 30px;
}

.tasting-form__field-location {
    flex: 1;
}

.tasting-form__button {
    width: 100%;
    background-color: transparent;
    border: 1px solid #fff;
    color: #fff;
    text-align: center;
    text-transform: uppercase;
    padding-top: 20px;
    padding-bottom: 20px;
    font-family: 'Montserrat';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 20px;
    letter-spacing: 0.05em;
}

.tasting-form__button:hover {
    cursor: pointer;
}

.tasting-form__button:active {
    box-shadow: 2px 2px 8px rgb(255, 255, 255, 0.3);
}

@media screen and (max-width: 1809px) {

    .tasting::before,
    .tasting::after {
        background-size: contain;
        background-repeat: no-repeat;
    }

    .tasting::before {
        width: 234px;
        height: 234px;
        top: -40px;
    }

    .tasting::after {
        width: 234px;
        height: 180px;
        right: -55px;
        top: -40px;
    }

    .tasting-form::before {
        content: "";
        width: 3px;
        height: 40px;
        background-color: #fff;
        display: block;
        position: absolute;
        left: -3px;
        top: -40px;
    }
}

@media screen and (max-width: 1739px) {
    .tasting::before {
        width: 208px;
        height: 208px;
        top: -40px;
    }

    .tasting::after {
        width: 208px;
        height: 160px;
        right: -46px;
        top: -22px;
    }

    .tasting-form::before {
        content: "";
        width: 3px;
        height: 40px;
        background-color: #fff;
        display: block;
        position: absolute;
        left: -3px;
        top: -40px;
    }

}

@media screen and (max-width: 1490px) {
    .tasting::before {
        top: -40px;
        left: -20px;

    }

    .tasting::after {
        right: -66px;
        top: -22px;
    }
}

@media screen and (max-width: 1490px) {

    .tasting__header-before,
    .tasting__header-after {
        display: none;
    }

    .tasting::after {
        right: -36px;
        top: -22px;
    }
}

@media screen and (max-width: 1024px) {
    .tasting::before {
        width: 182px;
        height: 182px;
        top: -22px;
        left: -22px;
    }

    .tasting::after {
        width: 182px;
        height: 140px;
        top: -14px;
    }
}

@media screen and (max-width: 968px) {
    .tasting::before {
        width: 156px;
        height: 156px;
        left: -28px;
    }

    .tasting::after {
        width: 156px;
        height: 120px;
    }
}

@media screen and (max-width: 768px) {
    .tasting::before {
        width: 130px;
        height: 130px;
        top: -12px;
    }

    .tasting::after {
        width: 130px;
        height: 100px;
        top: 0;
    }
}

@media screen and (max-width: 746px) {
    .content-wrapper {
        width: auto;
        padding: 0 35px;
    }
    .tasting__form {
        padding: 60px 0;
    }
    .tasting-form__client-info {
        flex-direction: column;
    }
    .tasting-form__field-name {
        margin-right: 0;
        margin-bottom: 40px;
    }
}

@media screen and (max-width: 706px) {
    .tasting::before,
    .tasting::after {
        display: none;
    }
    .tasting__text::before {
        margin: 25px auto;
    }
}

@media screen and (max-width: 507px) {
    .tasting__form::after {
        height: 120px;
        top: -120px
    }

    .tasting__form::before {
        height: 60px;
        top: -60px
    }
}
</style>