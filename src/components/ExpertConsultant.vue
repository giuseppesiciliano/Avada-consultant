<template>
    <div class="expert-consultant">

        <!-- Expert -->
        <img src="../assets/marketing-consultant-expert.jpg" alt="expert image">

        <div class="name">
            Richard Madsen
        </div>

        <div class="job">
            Marketing Consultant Expert
        </div>

        <div class="number">
            <i class="fa-solid fa-phone"></i> (555) 802-1234
        </div>

        <!-- Form Contact -->
        <form>
            <input type="text" placeholder="Your Name*">
            <input type="email" placeholder="Your Email*">
            <input type="number" placeholder="Your Phone Number*">
        </form>

        <!-- Button -->
        <div>
            <a class="button" href="#">Get a Callback</a>
        </div>

        <!-- Agree -->
        <span><a href="#">By submitting my data I agree to be contacted</a></span>
    </div>
</template>


<script>
export default {
  name: "ExpertConsultant",
}
</script>


<style lang="scss" scoped>
@import '../style/variables';
@import '../style/generals';

.expert-consultant {
    text-align: center;
    margin-left: 100px;
    height: 650px;
    width: 480px;

    border-radius: 15px;
    box-shadow: 0px 10px 10px #dedede;
    background-color: white;

    // Expert
    img {
        border-radius: 50%;
        width: 80px;
        padding: 30px 0
    }
    .name {
        font-size: 25px;
        padding-bottom: 20px;
    }
    .job {
        font-size: 18px;
        padding-bottom: 20px;
        color: grey;
    }
    .number {
        font-size: 18px;
        color: $primary-color;
    }

    // Form Contact
    form {
        display: flex;
        flex-direction: column;
        padding-top: 30px;

        input {
            padding: 20px;
            margin: 10px 20px;
            border-radius: 10px;
            border: 1px solid gray;
            font-size: 18px;
        }
    }
    .button {
        display: block;
        background-color: $primary-color;
        border-radius: 8px;
        padding: 20px 0;
        margin: 10px 20px;
        color: white;
    }
    .button:hover {
        background-color: #e9570b;
        transition: 0.2s;
    }
    span a {
        font-size: 15px;
        color: gray;
    }
}
</style>
