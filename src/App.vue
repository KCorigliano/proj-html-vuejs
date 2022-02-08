<template>
  <div id="app">
    <header-box 
      :headerLinks="headerLinks"
    />
    <jumbotron-box />
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    JumbotronBox
  },
  data() {
    return {
      headerLinks: [
        'Home',
        'Pages',
        'Courses',
        'Features',
        'Blog',
        'Shop',
      ],
      // headerLogo: '../assets/images/dark-logo.png',
    }
  },
}
</script>

<style lang="scss">
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
}
</style>
