<template>
    <section class="skills" id="skillsSide" >
        <h2>专业技能</h2>
        <ul class="clearfix">
            <li>
                <h3>HTML5<span>&</span>CSS</h3>
                <p>熟悉常见布局、盒模型、Flex、响应式、移动端适配，可快速根据设计稿开
                    发页面，熟悉开发调试，搭建符合 HTML5 语义化的页面结构</p>
                <div class="bar">
                    <div class="progressBar bar1"></div>
                </div>
            </li>
            <li>
                <h3>javaScript<span>&</span>jQuery</h3>
                <p>熟悉原生 JS，理解事件模型、原型、闭包、异步、面向对象、封装等，熟悉 AJAX、JSONP、跨域、
                    插件使用，了解 ES6 语法</p>
                <div class="bar">
                    <div class="progressBar bar2"></div>
                </div>
            </li>
            
            <li>
                <h3>框架</h3>
                <p>理解 MVC思想，熟悉 git 的使用进行版本管理，了解 Vue，可独立开发页面组件.</p>
                <div class="bar">
                    <div class="progressBar bar3"></div>
                </div>
            </li>
            
            <li>
                <h3>HTTP</h3>
                <p>了解 Http 通信原理，了解请求与响应的过程， 了解Cookie、Session、Cache-Control 等 HTTP 知识</p>
                <div class="bar">
                    <div class="progressBar bar4"></div>
                </div>
            </li>
        </ul>
	</section>

</template>


<script>
  
  export default {
    name:"page2",
    data(){
      return{
      }
    },
  };
</script>

<style>

/* .page2 { background:url(../img/bg3.jpg) no-repeat;background-position: center center;background-size: cover} */
.clearfix::after{content: '';display: block;clear: both;}

.skills{margin-top: 50px;}
section.skills,.portfolio{max-width: 940px;margin-left: auto;margin-right: auto;padding-top: 60px;}
.skills>h2{text-align: center;color: #fff;font-size: 34px;font-weight: 300;}

.skills>ul{box-shadow: 0px 3px 5px 0px rgba(0,0,0,0.3);padding: 42px 50px 10px;background: rgba(255, 255, 255, 0.1);
    margin-top: 30px;margin-top: 50px;}
.skills>ul>li{width: 47%;float: left;box-sizing: border-box;color: #ddd; }
.skills>ul>li>h3{font-size: 16px;color: #ccc;}
.skills>ul>li>h3>span{margin: 0 4px;}
.skills>ul>li>p{font-size: 12px;color: #eee;margin: 8px 0;}
.skills>ul>li:nth-child(even) {float: right;}
.skills>ul>li>h3{font-size: 14px;}
.skills>ul>li>.bar{background: #ced4e3;height: 5px;border-radius: 2px;margin: 6px 0 40px;overflow: hidden}
.skills>ul>li>.bar>.progressBar{height: 100%; width: 70%;background:#0adfd4;border-radius: 2px;transition: all 1s;}
.skills>ul>li>.bar>.progressBar.bar1{width: 80%}
.skills>ul>li>.bar>.progressBar.bar3{width: 60%}
.skills>ul>li>.bar>.progressBar.bar4{width: 40%}


</style>
