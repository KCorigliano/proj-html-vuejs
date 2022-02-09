<template>
<div class="container">
    <div class="row">
        <div class="img-box">
            <div class="bg-absolute-4"></div>
            <div class="bg-absolute-5"></div>
            <div class="bg-absolute-2">
                <svg xmlns="http://www.w3.org/2000/svg" width="200" height="202" fill="#1fad95"><path class="elementor-shape-fill" d="M139.374 198.088c16.328 8.906 51.35-1.087 58.304-39.038 7.15-39.022-13.182-40.052-9.633-54.248 14.243-21.15 16.782-48.14 2.028-64.387-36.503-38.024-45.629 7.604-76.048-20.28C101.727 7.837 83.1-6.735 56.23 3.405 18.239 17.74 27.33 47.659 27.33 69.313c0 7.624-24.216 21.957-26.87 41.573-3.346 24.734 12.168 57.29 26.87 68.443 23.322 26.363 59.318 20.28 75.541 11.154 13.931-7.836 25.35 1.52 36.503 7.605z"/></svg>
            </div>
            <div class="bg-absolute-3"></div>
            <img src="../../public/images/home-3-team-image.png" alt="">
            <div class="bg-absolute-1"></div>
        </div>
        <div class="text">
            <h4>EVERYTHING IN <span>MAXCOACH</span></h4>
            <h2>We're Here to <span>Transform</span> You</h2>
            <p>
                As learners, people can enjoy great companionship from
                MaxCoach mentors and educators. We can help your
                develop and grow at your best.
            </p>
            <button>Get Free Guide</button>
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
.row{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 150px;

    
    .text{
        width: 35%;

        h4{
            color: $stormDust;
            font-weight: 400;
            margin-bottom: 15px;
            span{
                font-weight: bold;
            }
        }

        h2{
            font-size: 50px;

            span{
                font-weight: 200;
                color: $montainMeadow;
            }
        }

        p{
            line-height: 25px;
            color: $stormDust;
            margin-top: 15px;
        }

        button{
            color: white;
            background-color: $montainMeadow;
            margin-top: 15px;
            padding: 15px 60px;
        }
    }

    .img-box{
        width: 60%;
        position: relative;

        .bg-absolute-4{
            position: absolute;
            height: 140px;
            width: 240px;
            bottom: -100px;
            right: 260px;
            z-index: -1;
            background: url('../../public/images/maxcoach-shape-07.png') no-repeat;
        }

        .bg-absolute-5{
            position: absolute;
            height: 140px;
            width: 240px;
            bottom: -70px;
            left: -290px;
            z-index: -1;
            background: url('../../public/images/maxcoach-shape-01.png') no-repeat;
        }

        .bg-absolute-2{
            position: absolute;
            top: 30px;
            left: -55px;
            z-index: -1;
            filter: opacity(40%);
        }

        .bg-absolute-3{
            position: absolute;
            height: 230px;
            width: 230px;
            top: 120px;
            left: -165px;
            z-index: -1;
            background: url('../../public/images/maxcoach-shape-05.png') no-repeat;
            background-size: cover;
        }

        img{
            border-radius: 5px;
        }

        .bg-absolute-1{
            position: absolute;
            height: 40px;
            width: 40px;
            top: -30px;
            right: -50px;
            border: 5px solid $drifwood;
            border-radius: 50%;
        }
    }
}
</style>