<template>
    <header>

        <!-- Logo -->
        <div class="logo">
            <a href="#">
                <img src="../assets/avada-marketing-logo.png" alt="logo AvadaConsultant">
            </a>
        </div>

        <!-- Menu -->
        <nav>
            <ul>
                <li v-for="(link, index) in linksArray" :key="index">
                    <a :href="link.url">
                        {{link.text}}
                    </a>
                </li>
            </ul>
        </nav>

        <!-- Servizi -->
        <div class="services">

            <ul>
                <li class="number">
                    <a href="#">
                        <i class="fa-solid fa-phone"></i>{{service}}
                    </a>
                </li>

                <li>
                    <a href="#">
                        <span class="secondary-button"> 
                            Free Quote
                        </span>
                    </a>
                </li>
            </ul>

        </div>
    </header>
</template>


<script>
export default {
  name: "Header",
  props: {
      linksArray: Array,
      service: String
  }
  
}
</script>


<style lang="scss" scoped>
@import '../style/variables';

header {
    display: flex;
    justify-content: center;
    align-items: center;

    height: 110px;

    ul {
        display: flex;
        
        li {
            padding-left: 30px;
            font-size: 19px;
            
            a {
                color: black;
                padding: 5px 10px;
            }
        }
    }
    nav a:hover {
        color: $primary-color;
        border-bottom: 2px solid $primary-color ;
    }
    .services {
        padding-left: 50px;
        font-size: 19px;

        i {
            color: $primary-color;
            padding-right: 18px;
        }
    }
}
</style>