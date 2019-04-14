<template>
    <section class="portfolio" id="portfolioSide">
        <h2>作品集</h2>
        <div class="items">
            <div class="item">
                <div class="description">
                    <h3>键盘导航</h3>
                    <p>可以根据自己的喜好设置网页导航，在键盘上按相应字母即可到达自己的网站</p>
                    <p>预览链接:<a href="https://cissypotato.github.io/Cissy-personal-nav/index.html" target="_blank">https://cissypotato.github.io/Cissy-personal-nav/index.html</a></p>
                    <p>代码链接:<a href="https://github.com/Cissypotato/Cissy-personal-nav" target="_blank">https://github.com/Cissypotato/Cissy-personal-nav</a></p>
                </div>

            </div>
            <div class="item">
                <div class="description">
                    <h3>canvas小画板</h3>
                    <p>用html5canvas API实现一个小画板，颜色、画笔大小可变换，可下载成图</p>
                    <p>预览链接:<a href="https://cissypotato.github.io/canvas/canvas.html" target="_blank">https://cissypotato.github.io/canvas/canvas.html</a></p>
                    <p>代码链接:<a href="https://github.com/Cissypotato/canvas" target="_blank">https://github.com/Cissypotato/canvas</a></p>
                </div>
            </div>
            <div class="item">
                <div class="description">
                    <h3>画一只皮卡丘</h3>
                    <p>用代码和动画的形式在网页上展现一个皮卡丘的形成过程，动画可调速</p>
                    <p>预览链接:<a href="https://cissypotato.github.io/Pikachu/index.html"target="_blank">https://cissypotato.github.io/Pikachu/index.html</a></p>
                    <p>代码链接:<a href="https://github.com/Cissypotato/Pikachu" target="_blank">https://github.com/Cissypotato/Pikachu</a></p>
                </div>
                
            </div>
            <div class="item">
                <div class="description">
                    <h3>手机版网易云音乐</h3>
                    <p>用 jQuery 实现 https://music.163.com/m/ （请用手机模式打开），mvc思想；rem实现自适应布局；leancloud和七牛云平台储存后台数据；</p>
                    <p>预览链接:<a href="https://cissypotato.github.io/163-music-1/src/index.html" target="_blank">https://cissypotato.github.io/163-music-1/src/index.html</a>（请用手机模式打开）</p>
                    <p>代码链接:<a href="https://github.com/Cissypotato/163-music-1" target="_blank">https://github.com/Cissypotato/163-music-1</a></p>
                </div>
            </div>
            <div class="item">
                <div class="description">
                    <h3>在线简历编辑</h3>
                    <p>用vue.js框架搭建页面，用vuex传送组件信息，用vue-router切换页面，使简历可在线保存，分享，更新，打印等</p>
                    <p>预览链接:<a href="https://cissypotato.github.io/vue-resume-4/index.html#/" target="_blank">https://cissypotato.github.io/vue-resume-4/index.html#/</a></p>
                    <p>代码链接:<a href="https://cissypotato.github.io/vue-resume-4" target="_blank">https://cissypotato.github.io/vue-resume-4</a></p>
                </div>
            </div>
            <div class="item">
                <div class="description">
                    
                    <h3>土豆翻译（微信小程序）</h3>
                    <p>一款简单的翻译小软件，可查看翻译历史以及更换7国语言</p>
                    <p>预览链接:微信小程序搜索“土豆翻译”</p>
                    
                </div>
            </div>
        </div>
    </section> 

</template>


<script>
  
  export default {
    name:"page3",
    data(){
      return{
      }
    },
  };
</script>

<style>

/* .page3 { background:url(../img/bg5.jpg) no-repeat;background-position: center center;background-size: cover} */

.portfolio{text-align: center;}
.portfolio>h2{text-align: center;color: #ddd;font-size: 34px;font-weight: 300;}
.portfolio>nav{display: inline-block;vertical-align: top;margin-top: 32px;}
.portfolio>nav>ol>li{float: left;margin-left: 30px;cursor: pointer;}
.portfolio>nav>ol>li:first-child{margin-left: 0;}
.portfolio>nav>.bar{height: 5px;border-radius: 2px;background: #fff;margin-top: 5px;}

.portfolio>.items{width: 100%;display: flex;flex-wrap: wrap;justify-content: space-between;margin-top: 50px;}
.items>.item{width: 420px;height:100px;margin-top: 20px;display: flex;
  padding:10px 5px;box-shadow: 0px 2px 4px 0px rgba(0,0,0,0.3); }
.item>.description{width: 100%;display: flex;flex-direction: column;justify-content: center}
.item>.description>h3{font-size: 14px;color: #fff;text-align: start;margin-left: 5px;}
.item>.description>p{font-size: 12px;color: #ccc;text-align: start;margin-left: 5px;margin-top: 5px;margin-bottom:0px;}
.item>.description>p>a{color: #eee;margin-left: 4px;}


</style>
