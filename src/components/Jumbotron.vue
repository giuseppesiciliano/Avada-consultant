<template>
  <div class="jumbotron">
    <div class="container">
      <div class="content">

        <!-- Area Text -->
        <div class="area-text">
          <h2>Unlock Your Online Growth Potential</h2>
          <p>Online Marketing to secure customer retention, leads, and sales. We focus on the bigger picture.</p>

          <a class="white-button" href="#">
            Our Services <i class="fa-solid fa-arrow-right"></i>
          </a>
        
        </div>

        <!-- Expert consultant -->
        <div class="expert-consultant">
          <ExpertConsultant />
        </div>
      </div>
    </div>
  </div>
</template>


<script>
import ExpertConsultant from "./ExpertConsultant.vue";

export default {
  name: "Jumbotron",
  components: {
    ExpertConsultant,
  },  
}
</script>


<style lang="scss" scoped>
@import '../style/variables';

.jumbotron {
  background-image: url('../assets/pexels-mikhail-nilov-7682340.jpg');
  background-repeat: no-repeat;
  background-position-y: top;
  background-size: cover;

  height: 700px;
  width: 100%;

  .content {
    padding-top: 120px;
    display: flex;
  }

  .area-text {
    color: white;
    width: 50%;

    h2 {
      font-size: 70px;
      font-weight: bold;
    }
    p {
      font-size: 30px;
      padding: 25px 0;
    }
    .white-button {
      margin-top: 15px;

      i {
        padding-left: 10px;
      }
    }
    .white-button:hover {
      background-color: rgba(0, 0, 0, 0);
      color: white;
      border: 1px solid white;
    }
  }

  .expert-consultant {
    padding-left: 50px;
    position: relative;
    top: -20px;
  }

  
}
</style>