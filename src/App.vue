<template>
  <div id="app">
    <Header :navLinks="navText"/>
    <Main/>
    <Footer :footerLinks="footerLinks"/>
    <FixedMenu/>
  </div>
</template>

<script>
import Header from './components/macro/Header.vue';
import Main from './components/macro/Main.vue';
import Footer from './components/macro/Footer.vue';
import FixedMenu from './components/commons/FixedMenu.vue';

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer,
    FixedMenu
  },
  data() {
    return {
      navText: [
        {
          title: 'Home',
          links: [
            'MaxCoach Education',
            'Course Portal',
            'Distant Learning',
            'Multimedia Pedagogy',
            'Modern Schooling',
            'Remote Training',
            'Health Coaching',
            'Gym Coaching',
            'Business',
            'Artist',
            'Kitchen Coach',
            'Motivation',
            'Dancing',
            'Guitar',
            'Yoga',
            'Photography',
            'Personal Finance'
          ]
        },
        {
          title: 'Pages',
          links: [
            'Start Here',
            'Success Story',
            'About me',
            'About us 01',
            'About us 02',
            'About us 03',
            'Contact me',
            'Contact us',
            'Purchase Guide',
            'Privacy Policy',
            'Terms of Service'
          ]
        },
        {
          title: 'Courses',
          links: [
            'Courses Grid 01',
            'Courses Grid 02',
            'Courses Grid 03',
            'Membership Levels',
            'Become a Teacher',
            'Profile',
            'Checkout',
            'Single Layout'
          ]
        },
        {
          title: 'Features',
          links: [
            'Events',
            'Zoom Meetings'
          ]
        },
        {
          title: 'Blog',
          links: [
            'Blog Grid',
            'Blog Masonry',
            'Blog Classic',
            'Blog List'
          ]
        },
        {
          title: 'Shop',
          links: [
            'Shop Left Sidebar',
            'Shop Right Sidebar',
            'Cart',
            'Wishlist',
            'Single Product'
          ]
        }
      ],
      footerLinks: [
        {
          title: 'Explore',
          links: [
            'Start here',
            'Success story',
            'Blog',
            'Courses',
            'About us',
            'Contact us'
          ]
        },
        {
          title: 'Information',
          links: [
            'Membership',
            'Purchase guide',
            'Privacy policy',
            'Terms of services'
          ]
        }
      ]
    }
  }
}
</script>

<style lang="scss">

@import './assets/style/global.scss'

</style>
