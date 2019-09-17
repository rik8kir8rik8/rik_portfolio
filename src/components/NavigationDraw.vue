<template>
  <div id="NavigationDraw">
  <div >
      <ul>
        <li><label v-scroll-to="'#works'" for="nav-input">WORKS</label></li>
        <li><a href="#feature"><label for="nav-input">WORKS</label></a></li>
        <li><a href="#about"><label for="nav-input">WORKS</label></a></li>
        <li><a href="#skill"><label for="nav-input">WORKS</label></a></li>
        <li><a href="#contact"><label for="nav-input">WORKS</label></a></li>
      </ul>
  </div>
  </div>
</template>

<script>

export default {
  name: 'NavigationDraw'
}
</script>
<style scoped>
#nav-input:checked ~ #nav-close {
  display: block;
  opacity: .5;
}

#nav-input:checked ~ #nav-content {
  -webkit-transform: translateX(15%);
  transform: translateX(15%);
  box-shadow: 6px 0 10px rgba(0,0,0,.25);
}
</style>
