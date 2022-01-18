<template>
    <div class="content">

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
                
            </div>
        </div>
    </div>
</template>


<script>
export default {
  name: "Leads", 
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
}
</style>