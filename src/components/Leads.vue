<template>
    <div class="container">

        <!-- Bar Consultant Expert -->
        <div class="bar">

            <!-- Profile -->
            <div class="profile">
                <img src="../assets/marketing-expert-cta.png" alt="marketing-expert-cta">

                <div class="name-job">
                    <div class="name">
                        Sandy Reiff
                    </div>

                    <div class="job">
                        Marketing Consultant Expert
                    </div>
                </div>
            </div>

            <!-- Title -->
            <h2>Drive Leads and Sales with Avada</h2>

            <!-- Number -->
            <a href="#">
                <span class="secondary-button"> 
                    <i class="fa-solid fa-phone"></i> (555) 802-1234
                </span>
            </a>
        </div>

        <!-- Leading Organisations -->
        <div class="lead-organisations">

            <h2 class="title-section">Trusted by Leading Organisations</h2>

            <div class="organisation-col">

                <!-- Singol Card -->
                <div v-for="(organisation, index) in organisation" :key="index" class="single-card">

                    <!-- Imagine -->
                    <div class="image">
                        <img :src="organisation.thumb" :alt="organisation.alt">
                        <div class="overlay"></div>
                    </div>

                    <!-- Title -->
                    <h3>{{organisation.title}}</h3>

                    <!-- Benefits -->
                    <div>{{organisation.benefit}}</div>
                    <span>{{organisation.subBenefit}}</span>
                </div>

            </div>

            <!-- Button -->
            <a class="primary-button" href="#">
                Read More Case Studies
            </a>
        </div>
    </div>
</template>


<script>
export default {
    name: "Leads",
    data: function() {
        return {
            organisation: [
                {
                    thumb: require('../assets/case-studies-1-400x450.jpg'),
                    alt: 'thumb organisation',
                    title: 'How Spaces attracted five million visitors by improving the content',
                    benefit: '200%',
                    subBenefit: 'Higher revenue from digital'
                },
                {
                    thumb: require('../assets/case-studies-4-400x450.jpg'),
                    alt: 'thumb organisation',
                    title: 'Creativity helped Hemisferio to increase their brand reach vertically',
                    benefit: '10x',
                    subBenefit: 'Sales increase with the same ad spend'
                },
                {
                    thumb: require('../assets/case-studies-6-400x450.jpg'),
                    alt: 'thumb organisation',
                    title: 'How DigitalBox used Al-powered data insight to boost sales',
                    benefit: '3-years',
                    subBenefit: 'Partnership with Avada Consultant'
                },
            ]
        }
    } 
}
</script>


<style lang="scss" scoped>
@import '../style/variables';
@import '../style/commons';

// Bar Consultant Expert
.bar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 10px 60px;

    margin: 150px 0;
    border-radius: 10px;
    box-shadow: 0px 10px 10px #dedede;

    // Profile
    .profile {
        display: flex;
        align-items: center;

        img {
            height: 80px;
            width: 80px;
            border-radius: 50%;
        }
        .name-job {
            padding-left: 30px;

            .name {
                font-size: 20px;
            }
            .job {
                padding-top: 5px;
                font-size: 14px;
            }
        }
    }
    

    // Title
    h2 {
        font-size: 25px;
    }

    // Number
    a {
        font-size: 20px;
        font-weight: bold;
    }
}

.lead-organisations {
    text-align: center;

    .organisation-col {
        display: flex;
        justify-content: space-around;

        .single-card {
            padding-top: 100px;
            text-align: left;
            width: 400px;

            h3 {
                font-size: 30px;
                padding: 20px 0;
            }
            h3::after {
                content: "";
                border: 1px dashed lightgray;
                margin-top: 20px;
                width: 100%;
                display: block;
            }
            div {
                font-size: 50px;
                font-weight: bold;
            }
            span {
                font-size: 18px;
            }
            .image {
                height: 450px;
                width: 400px;
                position: relative;

                img {
                    display: block;
                }
                .overlay {
                    transition: opacity 1s;
                    opacity: 0;
                    height: 100%;
                    width: 100%;
                    position: absolute;
                    top: 0;
                    left: 0;

                    background: rgb(255,145,27);
                    background: linear-gradient(0deg, rgba(214,93,0,0.6558998599439776) 40%, rgba(255,255,255,0) 94%);
                }
            }
            .image:hover .overlay {
                opacity: 1;
            }
        }
    }

    .primary-button {
        margin: 80px 0 130px 0;
    }
}
</style>