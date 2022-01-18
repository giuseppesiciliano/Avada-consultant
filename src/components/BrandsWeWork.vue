<template>
    <div class="brands-area">

        <h2 class="title-section">Some Brands We Work With</h2>

        <p class="p-section">Quisque aliquet, libero consequat elementum convallis</p>

        <ul class="brands-list">
            <li v-for="(brands, index) in brands" :key="index">
                <img :src="brands.thumb" :alt="brands.alt">
            </li>
        </ul>
    </div>
</template>


<script>
export default {
    name: "BrandsWeWork", 
    data: function() {
        return {
            brands: [
                {
                    name: 'abstract',
                    thumb: require('../assets/abstract.png'),
                    alt: 'logo abstract'
                },
                {
                    name: 'cglobal',
                    thumb: require('../assets/cglobal.png'),
                    alt: 'logo cglobal'
                },
                {
                    name: 'next',
                    thumb: require('../assets/next.png'),
                    alt: 'logo next'
                },
                {
                    name: 'hemisferio',
                    thumb: require('../assets/hemisferio.png'),
                    alt: 'logo hemisferio'
                },
                {
                    name: 'spaces',
                    thumb: require('../assets/spaces.png'),
                    alt: 'logo spaces'
                },
                {
                    name: 'digitalbox',
                    thumb: require('../assets/digitalbox.png'),
                    alt: 'logo digitalbox'
                }
            ]
        }
    }
}
</script>


<style lang="scss" scoped>
@import '../style/commons';

.brands-area {
    padding-top: 200px;
    text-align: center;

    p {
        padding-top: 20px;
    }

    ul {
        padding-top: 60px;
        display: flex;
        justify-content: center;

        li {
            padding: 0 30px;

            img {
                width: 140px;
            }
        }
    }
}
</style>