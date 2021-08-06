<template>
  <div id="app">
    <Drawer/>
    <Thumbnail/>
  </div>
</template>

<script>
import Drawer from './components/Drawer.vue'
import Thumbnail from './components/Thumbnail.vue'

export default {
  name: 'App',
  components: {
    Drawer,
    Thumbnail
  }
}
</script>