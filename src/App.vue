


<template>
  <div id="app">
    <!-- <img src="./assets/logo.png"> -->
    <div class="fullpage-container">
      <div class="fullpage-wp" v-fullpage="opts" ref="example">
        <div class="page-1 page">
          <div class="part-1" v-animate="{value: 'bounceInLeft'}">
            <page1></page1>
          </div>
        </div>


	


        <div class="page-2 page">
          <div class="part-2" v-animate="{value: 'bounceInRight'}">
            <page2></page2>
          </div>
        </div>


        <div class="page-3 page">
          <div class="part-3" v-animate="{value: 'bounceInRight'}">
            <page3></page3>
          </div>
        </div>

        <div class="page-4 page">
          <div class="part-4" v-animate="{value: 'bounceInRight'}">
            <page4></page4>
          </div>
        </div>

      </div>
      <button @click="moveNext">next</button>
    </div>
    <!-- <router-view/> -->
  </div>
</template>

<script>
import page1 from './components/page1.vue'
import page2 from './components/page2.vue'
import page3 from './components/page3.vue'
import page4 from './components/page4.vue'

export default {
  name: 'App',
  components:{
    page1,
    page2,
    page3,
    page4
  },
  data() {
    return {
      opts: {
        start: 0,
        dir: 'v',
        duration: 500,
        beforeChange: function (currentSlideEl,currenIndex,nextIndex) {
        },
        afterChange: function (currentSlideEl,currenIndex,nextIndex) {
        }
      }
    }
  },
  methods:{
    moveNext(){
      this.$refs.example.$fullpage.moveNext(); //Move to the next page
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  /* text-align: center; */
  /* color: #2c3e50;
  margin-top: 60px; */
}
.page-container {
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
}
.page-1 { background:url(http://ppyjs10p7.bkt.clouddn.com/bg1.jpeg) no-repeat;background-position: center center;background-size: cover}
.page-2 { background:url(http://ppyjs10p7.bkt.clouddn.com/bg3.jpg) no-repeat;background-position: center center;background-size: cover}
.page-3 { background:url(http://ppyjs10p7.bkt.clouddn.com/bg5.jpg) no-repeat;background-position: center center;background-size: cover}
.page-4 { background:url(http://ppyjs10p7.bkt.clouddn.com/bg4.jpg) no-repeat;background-position: center center;background-size: cover}

</style>
