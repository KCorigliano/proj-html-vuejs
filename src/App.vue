<template>
  <div id="app">
    <header-box 
      :headerLinks="headerLinks"
      :headerLogo="headerLogo"
    />
    <jumbotron-box />
    <main-container 
      :coursesCards="coursesCards"
      :blogsCards="blogsCards"
    />
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
      headerLogo: require('../public/images/dark-logo.png'),
      coursesCards:[
        {
            image: require('../public/images/course-02-480x298.jpg'),
            price: 40,
            title: 'Learning to Write as a Professional Author',
            lessons: 20,
            students: 50
        },
        {
            image: require('../public/images/stock-full-hd-03-480x298.jpg'),
            price: 0,
            title: 'Curstomer-centric info-Tech Strategies',
            lessons: 24,
            students: 769
        },
        {
            image: require('../public/images/stock-full-hd-04-480x298.jpg'),
            price: 19,
            title:  'Open Programming Courses fro Everyone: Python',
            lessons: 17,
            students: 62
        }
      ],
      blogsCards:[
        {
            image: require('../public/images/artist-blog-03-480x325.jpeg'),
            role: 'ARTIST',
            title: 'Brush Strokes Energize Trees in Paintings',
            date: 'May 15, 2020',
            views: '688 views'
        },
        {
            image: require('../public/images/artist-blog-01-480x325.jpg'),
            role: 'ARTIST',
            title: 'Pocket-Sized Notebooks Hold Miniature Paintings',
            date: 'May 15, 2020',
            views: '603 views'
        },
        {
            image: require('../public/images/artist-blog-02-480x325.jpg'),
            role: 'ARTIST',
            title:  'Connection Between Self-Portraits and Identity',
            date: 'May 15, 2020',
            views: '397 views'
        }
      ],
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
@import '@style/mainStyle.scss'
</style>
