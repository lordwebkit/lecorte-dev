<template>
    <div class="introduction">
        <h2 class="introduction__title">Лучший вкус, это вкус долголетнего вина</h2>
        <p class="introduction__text">
			На протяжении всего дня мы обращаемся к нашим пяти чувствам, сами того не осознавая: мы смотрим, слушаем, трогаем, чувствуем, пробуем.
            Рецепторы наших органов чувств реагируют на малейший возбудитель из окружающей среды, будь то запах, цвет, шум.
            Наши пять органов чувств: зрение, слух, обоняние, вкус и осязание, являются базой для дегустации.
            С их помощью мы можем понять, что хочет донести до нас вино (возраст, терруар, сепаж, условия хранения). 
            Прежде чем начать дегустацию, давайте зададим себе несколько вопросов: хорошо ли мы распознаем различные запахи?
            А вкусовые ощущения, такие как сладость, соленость, кислота, горечь? Сможем ли мы их различить? 
        </p>
        <div class="introduction__wine-wrapper">
            <img class="introduction__wine" src="../assets/wine-glass.png" alt="бокал для вина" />
        </div>
    </div>
</template>

<style scoped>
    .introduction {
        padding: 100px 60px 60px;
        border: solid #c4c4c4 3px;
    }

    .introduction__title,
    .introduction__text {
        color: #fff;
        text-align: center;
    }

    .introduction__title {
        font-size: 36px;
    }

    .introduction__title::after {
        display: block;
        width: 160px;
        height: 1px;
        background-color: #fff;
        content: "";
        margin: 40px auto;
    }

    .introduction__text {
        font-size: 15px;
        width: 70%;
        margin: 0 auto;
        margin-bottom: 100px;
    }

    .introduction__wine-wrapper {
        display: flex;
        justify-content: center;
    }

    @media screen and (max-width: 1440px) {
        .introduction__text {
            width: 90%;
        }
    }

    @media screen and (max-width: 1024px) {
        .introduction__text {
            width: 100%;
            text-align: justify;
        }
    }

    @media screen and (max-width: 768px) {
        .introduction {
            padding: 50px;
        }

        .introduction__text {
            margin-bottom: 40px;
        }
    }

    @media screen and (max-width: 692px) {
        .introduction__title {
            line-height: 1.2;
        }
    }

    @media screen and (max-width: 594px) {
        .introduction {
            padding-top: 30px;
        }
    }
</style>