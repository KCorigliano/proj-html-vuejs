<template>
<div class="container">
    <div class="row">
        <div class="text">
            <div class="title">
                <h4>EVERYTHING IN <span>MAXCOACH</span></h4>
            </div>
            <h2>Learn about our <span>Work Culture</span> at MaxCoach</h2>
            <p>
                Spend some time to visit our website or head office and
                discover our current courses, enrollment procedure, and
                registration deadline. We're opening new classes every
                beginning of each month.
            </p>
            <p>Have questions? <span>Get Free Guide →</span></p>
        </div>
        <div class="img-box">
            <img src="../assets/images/stock-full-hd-10-ohki1ayywq3cqutettrncduujpoaorifqu4relt2ts.jpg" alt="">
            <div class="bg-absolute-1"></div>
            <div class="bg-absolute-2"></div>
            <div class="bg-absolute-3"></div>
            <img class="img-absolute" src="../assets/images/about-us-01-ohkia3qg98rq9vg3s0mn2hkflr1migdqdw370qnegc.jpg" alt="">
            <img class="bg-absolute-4" src="../assets/images/maxcoach-shape-02.png" alt="">
        </div>
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

.container{
    padding-top: 150px;
    .row{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 150px;
    
        
        .text{
            width: 35%;
    
            h4{
                font-weight: 400;
                margin-bottom: 15px;
    
                span{
                    font-weight: bold;
                }
            }
    
            h2{
                font-size: 50px;
                span{
                    color: $montainMeadow;
                    font-weight: 200;
                }
            }
    
            p{
                line-height: 30px;
            }
    
            p:last-child{
                margin-top: 30px;
                span{
                    color: $montainMeadow;
                    padding-bottom: 5px;
                    text-decoration: underline;
                    font-weight: bold;
                    cursor: pointer;
                }
            }
        }
    
        .img-box{
            width: 50%;
            position: relative;
    
            img{
                border-radius: 5px;
            }
    
            .img-absolute{
                position: absolute;
                top: -100px;
                right: -40px;
            }
    
            .bg-absolute-1{
                position: absolute;
                height: 50px;
                width: 150px;
                top: -80px;
                right: 55px;
                background: url('../assets/images/maxcoach-shape-07.png');
                background-size: cover;
            }
    
            .bg-absolute-2{
                position: absolute;
                height: 30px;
                width: 130px;
                top: -30px;
                right: 65px;
                background: url('../assets/images/maxcoach-shape-07.png');
                background-size: cover;
            }
    
            .bg-absolute-3{
                position: absolute;
                height: 40px;
                width: 40px;
                top: -10px;
                left: -100px;
                border: 5px solid $drifwood;
                border-radius: 50%;
            }
    
            .bg-absolute-4{
                position: absolute;
                bottom: -90px;
                right: 85px;
            }
        }
    }
}

</style>