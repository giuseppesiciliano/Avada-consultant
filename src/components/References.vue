<template>
    <div class="content">
        <div class="container">

            <div class="scheda">

                <div class="text-area">
                    <h2 class="title-section">
                        We Boost Our Clients' Bottom Line by Optimizing Their Growth Potential.
                    </h2>

                    <p class="p-section">
                        Quisque aliquet, libero consequat elementum convallis, erat risus imperdiet pellentesque sem neque eget.
                    </p>

                    <a class="primary-button" href="#">
                        Why Work With Us
                    </a>
                </div>

                <img src="../assets/we-boost-our-clients-600x549.jpg" alt="">

            </div>

        </div>
    </div>
</template>

<script>
export default {
    name: "References",
}
</script>


<style lang="scss" scoped>
@import '../style/variables';
@import '../style/commons';

.content {
    background-color: #f5f5f7;

    width: 100%;

    .scheda {
        display: flex;
        justify-content: center;
        align-items: center;

        padding: 130px 0;

        .text-area {
            padding-right: 150px;
        }
        .p-section {
            padding: 30px 0;
        }
    }
}
</style>