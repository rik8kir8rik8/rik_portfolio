<template>
  <div id="pages">
  <top/>
  <works/>
  </div>
</template>

<script>
import top from './components/top.vue'
import works from './components/works.vue'
export default {
  name: 'pages',
  components: {
    top,
    works
  }
}
</script>

<style>

</style>
