<template>
  <div id="app" style="height: 100%;width: 100%;">
    <BoxStorage/>
  </div>
</template>

<script>
import BoxStorage from './components/BoxStorage'
export default {
  name: 'app',
  components: {
    BoxStorage,
  }
}
</script>

<style>
html{
  height: 100%;
  width: 100%;
}
</style>
