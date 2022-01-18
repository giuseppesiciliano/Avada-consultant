<template>
    <main class="container">
        
        <SingleRowBenefit v-for="(benefits, index) in benefits" :key="index" :benefitsArray="benefits" />
        <BrandsWeWork />
        <Leads />
    </main>
</template>


<script>
import SingleRowBenefit from "./SingleRowBenefit.vue";
import BrandsWeWork from "./BrandsWeWork.vue";
import Leads from "./Leads.vue";

export default {
  name: "Main", 
  components: {
    SingleRowBenefit,
    BrandsWeWork,
    Leads,
  },
  data: function() {
    return {
        benefits: [
            {
                logo: require('../assets/lo3.png'),
                icon: require('../assets/gg3.png'),
                upTitle: 'Business Growth',
                title: 'Increase Brand Awareness',
                subTitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa.',
                button: 'Get a Consultation',
                isReverse: false
            },
            {
                logo: require('../assets/lo2.png'),
                icon: require('../assets/gg2.png'),
                upTitle: 'Investors In People',
                title: 'In-House Sales Training',
                subTitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa.',
                button: 'Get a Consultation',
                isReverse: true
            },
            {
                logo: require('../assets/lo1.png'),
                icon: require('../assets/gg1.png'),
                upTitle: 'Social Media Analysis',
                title: 'Harness Your Social Proof',
                subTitle: 'Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed auctor placerat luctus. Nullam sit amet ante sed orci convallis gravida et at massa.',
                button: 'Get a Consultation',
                isReverse: false
            },
        ]
    }
  }
}
</script>


<style lang="scss" scoped>

</style>
