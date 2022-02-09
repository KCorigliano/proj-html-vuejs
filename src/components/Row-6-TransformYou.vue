<template>
<div class="row">
    <div class="img-box">
        <img src="../assets/images/home-3-team-image.png" alt="">
    </div>
    <div class="text">
        <h2>We're Here to Transform You</h2>
        <p>
            As learners, people can enjoy great companionship from
            MaxCoach mentors and educators. We can help your
            develop and grow at your best.
        </p>
        <button>Get free guide</button>
    </div>
</div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.row{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 150px;

    
    .text{
        width: 35%;

        h2{
            font-size: 50px;
        }
    }

    .img-box{
        width: 60%;
        position: relative;

        img{
            border-radius: 5px;
        }
    }
}
</style>