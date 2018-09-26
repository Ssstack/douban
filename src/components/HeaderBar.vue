<template>
    <div class="header-bar">
        <header>
            <div class="logo">
                <router-link to="/">
                    <h1>豆瓣</h1>
                </router-link>
            </div>
            <nav>
                <ul>
                    <li>
                        <router-link to="/movie">电影</router-link>
                    </li>
                    <li>
                        <router-link to="/book">图书</router-link>
                    </li>
                    <li>
                        <router-link to="/status">广播</router-link>
                    </li>
                    <li>
                        <router-link to="/group">小组</router-link>
                    </li>
                </ul>
                <div class="search-btn" @click="showTalion">
                    <img src="../assets/search-btn.png">
                </div>
            </nav>
        </header>
    </div>
</template>

<script>
export default {
    methods: {
        showTalion() {
            
        }
    }
}
</script>

<style lang="scss" scoped>
.header-bar {

    header {
        margin: 0 auto;
        padding: 0 18px;
        height: 47px;
        line-height: 47px;
        border-bottom: 1px solid #eee;
        .logo {
            float: left;
            h1 {
                margin: 0;
                color: #00b600;
                font-size: 1.5em;
            }
        }
        nav {
            float: right;
            overflow: hidden;
            ul {
                float: left;
                overflow: hidden;
                li {
                    float: left;
                    margin-right: 19px;
                    font-size: 15px;
                    &:first-of-type {
                        a {
                            color: #2384E8;
                        }
                    }
                    &:nth-of-type(2) {
                        a {
                            color: #9F7860;
                        }
                    }
                    &:nth-of-type(3) {
                        a {
                            color: #E4A813;
                        }
                    }
                    &:last-of-type {
                        a {
                            color: #2AB8CC;
                        }
                    }
                }
            }
            .search-btn {
                float: left;
                margin-top: 16px;
                width: 24px;
                height: 18px;
                img {
                    width: 100%;
                }
            }
        }
    }
}
 
</style>