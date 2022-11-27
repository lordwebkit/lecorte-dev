<script>
    export default {
        data() {
            return {
                navBarList: [
                    {name: 'Каталог', link: '#collection'},
                    {name: 'Доставка', link: '#'},
                    {name: 'Коллекции', link: '#'},
                    {name: 'Контакты', link: '#footer'},
                ]
            }
        }
    }
</script>
<template>
    <nav class="nav-bar">
        <a v-for="navBarItem in navBarList" :href="navBarItem.link" class="nav-bar__button-wrapper">
            <p class="nav-bar__button">{{navBarItem.name}}</p>
        </a>
    </nav>
</template>

<style scoped>
    .nav-bar {
        display: flex;
        height: 45px;
    }

    .nav-bar__button {
        color: #fff;
        text-align: center;
        flex: 1;
        font-size: 14px;
        line-height: 150%;
    }

    .nav-bar__button-wrapper {
        flex: 1;
        align-items: center;
        display: flex;
        border: solid #fff 1px;
        border-left: none;
        text-decoration: none;
    }

    .nav-bar__button-wrapper:last-child {
        border-right: none;
    }

    .nav-bar__button-wrapper:hover {
        background-color: rgba(255, 255, 255, 0.089);
    }

    .nav-bar__button-wrapper:active {
        background-color: rgba(0, 0, 0, 0.123);
    }


    .nav-bar__button-wrapper:visited .nav-bar__button{
        text-decoration: none;
    }

    @media screen and (max-width: 670px) {
        .nav-bar {
            display: none;
        }
    }
</style>