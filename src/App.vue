<template>
  <div id="app">
    <header-box 
      :headerLinks="headerLinks"
    />
    <jumbotron-box />
    <main-container />
    <footer-box 
      :exploreLinks="exploreLinks"
      :informationLinks="informationLinks"
    />
  </div>
</template>

<script>
import HeaderBox from './components/HeaderBox.vue'
import JumbotronBox from './components/JumbotronBox.vue'
import MainContainer from './components/MainContainer.vue'
import FooterBox from './components/FooterBox.vue'

export default {
  name: 'App',
  components: {
    HeaderBox,
    JumbotronBox,
    MainContainer,
    FooterBox
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
      exploreLinks:[
        'Start here',
        'Blog',
        'About us',
        'Success story',
        'Courses',
        'Contact us',
      ],
      informationLinks:[
        'Membership',
        'Purchase guide',
        'Privacy policy',
        'Terms of service',
      ]
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
