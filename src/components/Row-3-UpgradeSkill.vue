<template>
<div class="container">
    <div class="row">
        <div class="img-box">
            <div class="bg-absolute-1"></div>
            <div class="bg-absolute-2">
                <img src="../assets/images/svg-0.svg" alt="">
            </div>
            <div class="bg-absolute-3"></div>
            <img src="../assets/images/stock-full-hd-11-670x450.jpg" alt="">
            <img class="youtube-logo" src="../assets/images/icon-youtube-play.png" alt="">
        </div>
        <div class="text">
            <h4>HOW WE WORK</h4>
            <h2>Upgrade Your Skills <span>Upgrade Your Life</span></h2>
            <p>
                Opening up more opportunities in fron of your to get the
                ticket to more enjoyable door in life. Getting equipped with 
                new skills for new sets of insights into your career.
                MaxCoach accompany learners in every stage of learning.
            </p>
            <p>Download free guidebook →</p>
        </div>
        <div class="bg-absolute"></div>
    </div>
</div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/mainStyle.scss';
.row{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 75px;
    position: relative;

    .img-box{
        width: 60%;
        position: relative;

        .bg-absolute-1{
            position: absolute;
            height: 140px;
            width: 140px;
            bottom: -61px;
            right: 25px;
            z-index: -1;
            background: url('../assets/images/maxcoach-shape-07.png');
        }

        .bg-absolute-2{
            position: absolute;
            top: -90px;
            left: -65px;
            z-index: -1;

            img{
                filter: invert(80%);
            }
        }

        .bg-absolute-3{
            position: absolute;
            height: 190px;
            width: 140px;
            top: 55px;
            left: -95px;
            z-index: -1;
            background: url('../assets/images/maxcoach-shape-05.png') no-repeat;
        }
    }

    .youtube-logo{
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
    }

    .text{
        width: 35%;

        h4{
            font-weight: 400;
            margin-bottom: 15px;
        }

        h2{
            font-size: 50px;
            margin-bottom: 15px;
            span{
                color: $montainMeadow;
                font-weight: 400;
            }
        }

        p{
            line-height: 25px;
            color: $stormDust;
        }

        p:last-child{
            line-height: 25px;
            margin-top: 30px;
            color: black;
            text-decoration: underline;
            font-weight: bold;
            cursor: pointer;
        }
    }

    .bg-absolute{
        position: absolute;
        height: 40px;
        width: 40px;
        top: -25px;
        right: 395px;
        border: 5px solid $drifwood;
        border-top-color: $quillGray;
        border-radius: 50%;
    }
}
</style>