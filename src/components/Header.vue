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
            <i class="fa-solid fa-phone"></i>{{service}}
        </div>
    </header>
</template>


<script>
export default {
  name: "Header",
  props: {
      linksArray: Array,
      service: Object
  }
  
}
</script>


<style lang="scss" scoped>
header {
    display: flex;
    justify-content: center;
    align-items: center;

    height: 100px;
    background-color: pink;

    nav ul {
        display: flex;
        
        li {
            padding-left: 40px;
            font-size: 19px;
            
            a {
                color: black;
            }
        }
    }

    .services {
        padding-left: 50px;
        font-size: 19px;

        i {
            color: #f86011;
            padding-right: 18px;
        }
    }
}
</style>