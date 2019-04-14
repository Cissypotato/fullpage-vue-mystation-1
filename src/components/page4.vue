<template>
    <div>
        <section class="experience"  >
            <h2>工作经历</h2>
            <div>
                <p> <span class="time">201707-201807</span> <span>上海黍家科技有限公司</span> <span>电商美工</span></p><span></span>
                <p> <span class="time">201803-至今</span> <span>自学前端</span></p>
            </div>
                
        </section>
        <section class="message" id="message" >
            <h2>留言</h2>
            <div>
                <ol id="messageList"></ol>
                <form action="" id="postMessageForm" style="width:700px;margin:50px auto;">
                    <label>姓名：</label>
                    <input type="text"name="name" class="name">
                    <label>留言：</label>
                    <input type="text"name="content"  class="content">
                    <button type="submit" class="submit">提交</button>
                </form>
            </div>
            
        </section>
        <!-- footer -->
        <footer>
            <p>©Cissy || 2017-2018</p>
        </footer>
    </div>

</template>

<script src="//cdn1.lncld.net/static/js/3.6.8/av-min.js"></script>
<script>
  
  export default {
    name:"page4",
    data(){
      return{
      }
    },
    methods:{
        init:function(){
            var APP_ID = 'ccFrNOWfVvznB3jVaAR3D9LS-gzGzoHsz';
            var APP_KEY = 'bJNJepBXn0L3lssSqv03zgaE';
            AV.init({appId: APP_ID,appKey: APP_KEY});
        },
    }
  };
</script>

<style>

/* .page4 { background:url(../img/bg4.jpg) no-repeat;background-position: center center;background-size: cover} */


.experience{margin-top: 160px;display: flex;justify-content: center;width: 80%;}
.experience>h2{text-align: center;color: #ddd;font-size: 20px;font-weight: 300;width: 30%;margin-top: 10px;}
.experience>div{width:70%}
.experience>div>p{margin-top: 10px;background: rgba(255,255,255,0.1);padding: 4px 8px;color: #ddd}
.experience>div>p>span.time{width: 30%;display: inline-block}
/*message*/
.message{margin-top: 100px;display: flex;width: 80%;}
.message>h2{text-align: center;color: #ddd;font-size: 20px;font-weight: 300;width: 30%}
.message>div{width:70%}
.message>div>ol{background: rgba(255,255,255,0.1);padding: 20px 30px;}
.message>div>ol>li{padding-top: 16px;padding-bottom: 3px;padding-left: 16px;;border-bottom: 1px solid  rgb(82, 3, 26);color: #ccc}
.message>div>form>label{color: rgb(44, 2, 14)}
input.name{background: none;border: none;border-bottom: 1px solid rgb(82, 3, 26);margin-right: 100px;}
input.name:focus{outline: none;background-color: none;}
input.content{background: none;border: none;border-bottom: 1px solid rgb(82, 3, 26);margin-right: 100px;}
input.content:focus{outline: none;background-color: none;}
button.submit{color: #ddd;background:rgba(255, 255, 255,0.1);border: none;padding: 4px 8px;cursor: pointer;border-radius: 2px;}


/*footer*/
footer>p{text-align: center;color: rgb(82, 3, 26);margin: 20px;font-size: 14px;}


</style>
