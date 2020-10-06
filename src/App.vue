<template>
  <div id="app">
    <edit-field/>
  </div>
</template>

<script>
import EditField from '@/components/EditField'

export default {
  name: 'App',
  components: {
    EditField
  }
}
</script>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
