<template>
    <div class="home">
        <div class="nav">
            <header-bar></header-bar>
        </div>
        <div class="main">
            <home-page></home-page>
        </div>
    </div>
</template>

<script>
// 把其他组件引入当前页然后使用
import HeaderBar from '../components/HeaderBar';
import HomePage from './HomePage.vue';

export default {
    name: 'home',
    components: {
        // 注册
        HeaderBar,
        HomePage
    },
    data() {
        return {

        }
    },
    methods: {

    }
}
</script>

<style lang="scss" scoped>
    .home {
        max-width: 650px;
        min-width: 320px;
        margin: 0 auto;
        .nav {
            position: fixed;
            top: 0;
            left: 50%;
            z-index: 999;
            transform: translateX(-50%);
            max-width: 650px;
            min-width: 320px;
            width: 100%;
            background-color: #fff;
        }
        .main {
            max-width: 650px;
            min-width: 320px;
        }
    }
</style>