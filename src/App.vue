<template>
  <div id="app">

    <Header :linksArray="links" :service="callService"/>
    <Jumbotron />
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Jumbotron from "./components/Jumbotron.vue";

export default {
  name: "App",
  components: {
    Header,
    Jumbotron,
  },
  data: function() {
    return {
      links: [
        {
          text: 'Home',
          url: '#'
        },
        {
          text: 'Services',
          url: '#'
        },
        {
          text: 'Why Us',
          url: '#'
        },
        {
          text: 'Case Studies',
          url: '#'
        },
        {
          text: 'About',
          url: '#'
        },
        {
          text: 'Blog',
          url: '#'
        }
      ],
      callService: '(555) 802-1234'
    }
  },
};
</script>

<style lang="scss">
@import './style/generals';
@import './style/commons';

</style>
