<template>
    <div class="home-page">
        <div class="quick-nav">
            <ul>
                <li>
                    <a href="">影院热映</a>
                </li>
                <li class="dynamic">
                    <a href="">近期值得看的美剧</a>
                </li>
                <li>
                    <a href="">豆瓣时间</a>
                </li>
                <li>
                    <a href="">使用豆瓣App</a>
                </li>
            </ul>
        </div>
        <div class="recommend">
            <a href="" class="rec-item">
                <div class="content">
                    <div class="pic">
                        <img src="../assets/story.jpg">
                    </div>
                    <h3>我心目中的爱情电影十佳名单。</h3>
                    <p>姐妹篇? &lt;那些或甜或咸的爱情的歌&gt; https://www.douban.com/note/690916989/ 作为一个城市人。 作为一个在城市多年打拼毫无起色的城市人。真的是有大把的时间来花在电影和电视剧上。但是也不敢说是有多么的资深。 还记得半个月前，朋友圈里刮起来的一股子风潮，网易云音乐一套荣格心理学的测试题纷纷扰扰的，占领了整个朋友圈。我呢，一个外在【战士】内在【孤儿】，按页面说这样的组合只占3%的人，应该算是有一点独特的。再加上长久以来，各种心理测试都说什么，心里年纪32...</p>
                </div>
                <div class="author">
                    by
                    <span class="name">Theo</span>
                </div>
            </a>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.home-page {
    margin: 0 18px;
    padding-top: 47px;
    .quick-nav {
        ul {
            margin-top: 20px;
            font-size: 14px;
            line-height: 44px;
            text-align: center;
            overflow: hidden;
            li {
                float: left;
                width: 50%;
                padding: 3px;
                box-sizing: border-box;
                a {
                    display: block;
                    width: 100%;
                    background-color: #f6f6f6;
                }
            }
        }
    }
    .recommend {
        .rec-item {
            position: relative;
            display: block;
            padding: 25px 0;
            box-sizing: border-box;
            &:after {
                content: '';
                position: absolute;
                left: 0;
                bottom: 0;
                width: 100%;
                height: 1px;
                transform: scaleY(0.5);
                background-color: #e3e3e3;
            }
            .content {
                margin-bottom: 10px;
                overflow: hidden;
                 h3 {
                    margin-bottom: 6px;
                    font-weight: 400;
                    font-size: 17px;
                    line-height: 1.4;
                    color: #494949;
                }
                .pic {
                    float: right;
                    margin-left: 25px;
                    width: 25%;
                }
                p {
                    font-weight: 400;
                    font-size: 12px;
                    line-height: 1.5;
                    color: #aaa;
                    display: -webkit-box;
                    overflow: hidden;
                    -webkit-box-orient: vertical;
                    -webkit-line-clamp: 3;
                }
            }
            .author {
                font-size: 12px;
                color: #ccc;
            }
        }
    }
}
</style>

