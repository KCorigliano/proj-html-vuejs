<template>
   <div class="row">
            <div class="img-box">
                <img src="../assets/images/stock-full-hd-11-670x450.jpg" alt="">
                <img class="youtube-logo" src="../assets/images/icon-youtube-play.png" alt="">
            </div>
            <div class="text">
                <h2>Upgrade Your Skills Upgrade Your Life</h2>
                <p>
                    Opening up more opportunities in fron of your to get the
                    ticket to more enjoyable door in life. Getting equipped with 
                    new skills for new sets of insights into your career.
                    MaxCoach accompany learners in every stage of learning.
                </p>
                <p>Download free guidebook</p>
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

    .img-box{
        width: 60%;
        position: relative;
    }

    .youtube-logo{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    .text{
        width: 35%;
    }
}
</style>