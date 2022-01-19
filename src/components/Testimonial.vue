<template>
    <div class="container">
        <section>

            <img src="../assets/large-testimonial-600x583.jpg" alt="testimonial">

            <div class="area-text">

                <h2 class="quote">
                    "The team at Avada Marketing Consultant is fabulous. They helped us unlock our potential online and offline. We have experienced year on year growth due to their progressive approach."
                </h2>

                <span class="name">
                    Kate Schadler
                </span>

                <span class="job">
                    Marketing Consultant - Abstract
                </span>

            </div>

        </section>
    </div>
</template>


<script>
export default {
    name: "Testimonial",
}
</script>


<style lang="scss" scoped>
section {
    display: flex;
    align-items: center;
    padding: 100px 0;

    img {
        border-radius: 10px;
    }

    .area-text {
        padding-left: 120px;
        display: flex;
        flex-direction: column;

        .quote {
            font-size: 30px;
            line-height: 45px;
            padding-bottom: 50px;
        }
        .name {
            font-size: 17px;
            font-weight: bold;
            padding-bottom: 15px;
        }
        .job {
            font-size: 12px;
        }
    }
}
</style>