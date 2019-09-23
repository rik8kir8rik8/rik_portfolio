<template>
  <div id="app">
    <Navigation/>
    <div class="box-sub">
    <illustration/>
    </div>
    <div class="box-main">
      <top/>
      <skills/>
    </div>
    <div class="box-bottom">
    <profile/>
    </div>
  </div>
</template>

<script>
import Navigation from './components/Navigation.vue'
import top from './components/top.vue'
import profile from './components/profile.vue'
import skills from './components/skills.vue'
import illustration from './components/illustration.vue'

import Vue from "vue"
import VueScrollTo from 'vue-scrollto'

Vue.use(VueScrollTo, {
  offset: -100,
});

export default {
  name: 'app',
  components: {
    Navigation,
    top,
    profile,
    skills,
    illustration
  },
  function(ctx, inject) {
  inject("scrollTo", VueScrollTo.scrollTo);
}
}
</script>

<style lang="scss">
    @media screen and (min-width: 600px) {
        #app {
    padding-left:20%;
    padding-right:20%;
    padding-top:5%;
  }
  .box-main, .box-sub {
  float: left;
  width: 50%;
  padding-top:10%;
  }
    }
    @media screen and (max-width: 600px) {
        #app {
    padding-left:20%;
    padding-right:20%;
    padding-top:5%;
  }
    .box-sub{
      float:left;
    }
    .box-main{
      padding-top:20%;
      width:100%;
    }
  }
  @media screen and (max-width: 480px) {
    .box-sub{
      margin-top:70%;
    }
    .box-main{
      padding-top:20%;
      width:100%;
    }
  }
  .box-bottom{
  float: left;
  width: 100%;
  }
</style>
