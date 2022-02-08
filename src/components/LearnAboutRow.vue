<template>
<div class="row">
    <div class="text">
        <h2>Learn about our Worl Culture at MaxCoach</h2>
        <p>
            Spend some time to visit our website or head office and
            discover our current courses, enrollment procedure, and
            registration deadline. We're opening new classes every
            beginning of each month.
        </p>
        <p>Have questions? Get Free Guide</p>
    </div>
    <div class="img-box">
        <img src="../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">
        <img class="img-absolute" src="../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
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

        .img-absolute{
            position: absolute;
            top: -100px;
            right: 80px;
        }
    }
}
</style>