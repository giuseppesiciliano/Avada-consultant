<template>
  <div id="app">

    <Header :linksArray="links" :service="callService"/>
    <Jumbotron :expert="expertConsultant" />
    <Row />
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
          url: '#',
          dropDown: true
        },
        {
          text: 'Services',
          url: '#',
          dropDown: true
        },
        {
          text: 'Why Us',
          url: '#',
          dropDown: false
        },
        {
          text: 'Case Studies',
          url: '#',
          dropDown: false
        },
        {
          text: 'About',
          url: '#',
          dropDown: false
        },
        {
          text: 'Blog',
          url: '#',
          dropDown: false
        }
      ],
      callService: '(555) 802-1234',
      expertConsultant: {
        img: '../assets/marketing-consultant-expert.jpg',
        name: 'Richard Madsen',
        job: 'Marketing Consultant Expert',
        number: '(555) 802-1234',
      }
    }
  },
};
</script>

<style lang="scss">
@import './style/generals';
@import './style/commons';

</style>
