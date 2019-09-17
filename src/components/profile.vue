<template>
    <footer id="profile">
      <selecter class="icon"></selecter>
        <h1>profile</h1>
        <h2>Risako Kikuchi</h2>
        <p>1994/8/16 Live in Japan.</p>
    </footer>
</template>

<script>
export default {
  name: 'profile',
  components: {
  }
}
</script>

<style lang="scss">

@media screen and (min-width: 600px) {
     #profile{
    width: 100%;
    height:15rem;

  .box-main, .box-sub {
  float: left;
  width: 50%;
  padding-top:10%;
  }
     }
 }

  @media screen and (max-width: 600px) {
      #profile{
    width: 100%;
    height:15rem;
  .box-main, .box-sub {
  float: left;
  width: 50%;
  padding-top:10%;
  }
      }
 }

 @media screen and (min-width: 600px) {
      #profile{
    width: 100%;
    height:15rem;
  .box-main, .box-sub {
  float: left;
  width: 50%;
  padding-top:10%;
  }
      }
 }
</style>

