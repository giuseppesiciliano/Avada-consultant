<template>
  <div id="app">

    <Header :linksArray="links" :service="callService"/>
  </div>
</template>

<script>
import Header from "./components/Header.vue";

export default {
  name: "App",
  components: {
    Header,
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

</style>
