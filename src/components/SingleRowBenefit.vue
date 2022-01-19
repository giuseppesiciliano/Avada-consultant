<template>
    <div class="container">
        <div class="row" :class="{'reverse' :benefitsArray.isReverse}">
        
            <!-- Logo -->
            <div class="logo-area">
                <img :src="benefitsArray.logo" alt="logo 1">
            </div>

            <!-- Area Text -->
            <div class="text-area">
        
                <img :src="benefitsArray.icon" alt="">

                <span>{{benefitsArray.upTitle}}</span>
        
                <h3>{{benefitsArray.title}}</h3>

                <p class="p-section">{{benefitsArray.subTitle}}</p>

                <a class="primary-button" href="#">
                    {{benefitsArray.button}}
                </a>
            </div>
            
        </div>
    </div>
</template>


<script>
export default {
  name: "SingleRowBenefit", 
  props: {
    benefitsArray: Object
  }
}
</script>


<style lang="scss" scoped>
.row {
    display: flex;
    align-items: center;
    
    padding-top: 230px;

    .logo-area {
        padding-right: 230px;
    }

    .text-area {

        img {
            vertical-align: middle;
        }
        span {
            font-size: 20px;
            padding-left: 20px;
        }
        h3 {
            font-size: 50px;
            padding: 20px 0;
        }
        p {
            padding-bottom: 25px;
        }
    }
}

.reverse {
    flex-direction: row-reverse;

    .logo-area {
        padding-right: 0;
        padding-left: 230px;
    }
}
</style>