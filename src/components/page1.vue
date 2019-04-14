<template>
    <div>
        <div class="header">
            <P class="logo"><span class="rs">R</span><span class="card">esume</span></P>
            <div class="blogAndGithub">
                <a href="https://www.jianshu.com/u/5c61e896610e" target="_blank" >博客</a>
                <a href="https://github.com/Cissypotato" target="_blank" >github</a>							
                <a class="downloadResume" href="./前端开发_陈茜_四川农业大学_13881739295.pdf" target="_blank" download>下 载 PDF 文 档</a>						
            </div>
        </div>
        <div class="about">
            <div class="avatarWrapper">
                <div class="avatar"></div>						
            </div>
            <h3>陈茜</h3>
            <div class="abItem">						
                <svg class="icon occupation" aria-hidden="true">
                <use xlink:href="#icon-xiaogegeyizhuanhuan_zhiye"></use>
                </svg>
                求职意向  前端开发工程师								
            </div>
            <div class="abItem">						
                <svg class="icon" aria-hidden="true">
                <use xlink:href="#icon-weixin1"></use>
                </svg>
                c1395422644		
            </div>
            <div class="abItem">
                <svg class="icon" aria-hidden="true">
                    <use xlink:href="#icon-youxiang"></use>
                </svg>
                1395422644@qq.com
            </div>
            <div class="abItem">
                <svg class="icon" aria-hidden="true">
                    <use xlink:href="#icon-jiaoyu1"></use>
                </svg>
                四川农业大学(2013/2017) 景观建筑设计 CET6过
            </div>
        </div>
    </div>

</template>


<script>
  
  export default {
    name:"page1",
    data(){
      return{
      }
    },
  };
</script>

<style scoped>

/* .page1 { background:red;background-position: center center;background-size: cover} */
.header{width: 100%;display: flex;justify-content: space-between}
.logo{font-family:"Arial Black";margin: 20px;}
.logo .rs{font-size: 24px;padding-right: 5px;color:#84a3eb;}
.logo .card{font-size: 24px;color:#bbb;}
.blogAndGithub{margin: 20px;}
.blogAndGithub>a{padding: 0 20px;line-height:33px;color: #ccc;font-size: 14px;}
a.downloadResume{display: inline-block;font-size: 12px;
    padding: 2px 12px;transition: box-shadow 0.8s; }
a.downloadResume:hover{box-shadow: 0px 7px 16px 0px rgba(77,96,139,0.65);}

.about{display: flex;flex-direction: column;justify-content: center;align-items: center;color: #ddd;margin-top: 20px;}
.avatarWrapper{display: flex;justify-content: center;align-items:top;flex-direction: column;align-items: center;}
.avatarWrapper>.avatar{width: 150px;height: 150px;border: 3px solid #fff;border-radius: 50%;
    background: url(http://ppyjs10p7.bkt.clouddn.com/avatar5.jpg) center center no-repeat;background-size: cover;box-shadow: 0px 7px 16px 0px rgba(77,96,139,0.65) ;}
.about>h3{margin-top:40px;font-size: 40px;font-weight: 500;margin-bottom: 20px;}
.abItem{padding: 5px 10px ;background: rgba(255,255,255,0.1);margin-top: 8px;width: 40%;text-align: center;
    display: flex;align-items: center;justify-content: center}
.abItem>div{margin: 0 auto;width: 50%;}
.abItem>svg.icon{margin-right: 10px;width: 20px;height: 20px;}
.abItem>svg.icon.occupation{width: 22px;height: 22px;fill: #eee}
</style>
