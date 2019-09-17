<template>
  <div id="app">
    <Navigation/>
    <div class="box-sub">
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
    skills
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
    padding-top:10%;
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
      display:none;
    }
    .box-main{
      padding-top:20%;
      width:100%;
    }
  }
  @media screen and (max-width: 479px) {
    .box-sub{
      display:none;
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
