<template>
    <div class="container">
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
        <div class="curiosity-row">
            <div>
                <h1>129+</h1>
                <p>Enrolled learners</p>
            </div>
            <div>
                <h1>80</h1>
                <p>Finished sessions</p>
            </div>
            <div>
                <h1>4%</h1>
                <p>Satisfaction rate</p>
            </div>
        </div>
        <div class="row">
            <div class="img-box">
                <img src="../assets/images/stock-full-hd-11-670x450.jpg" alt="">
                <!-- <img class="youtube-logo" src="../assets/images/icon-youtube-play.png" alt=""> -->
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
        <div class="row">
            <h1>Latest Online Courses</h1>
        </div>
        <div class="row">
            <div class="courses-container">
                <img src="../assets/images/course-02-480x298.jpg" alt="">
                <div class="courses-text">
                    <h2>$40.00</h2>
                    <p>Learning to Write as a Professional Author</p>
                    <div>
                        <span>20 Lessons</span>
                        <span>50 Students</span>
                    </div>
                </div>
            </div>
            <div class="courses-container">
                <img src="../assets/images/stock-full-hd-03-480x298.jpg" alt="">
                <div class="courses-text">
                    <h2>$0.00</h2>
                    <p>Curstomer-centric info-Tech Strategies</p>
                    <div>
                        <span>24 Lessons</span>
                        <span>769 Students</span>
                    </div>
                </div>
            </div>
            <div class="courses-container">
                <img src="../assets/images/stock-full-hd-04-480x298.jpg" alt="">
                <div class="courses-text">
                    <h2>$19.00</h2>
                    <p>Open Programming Courses fro Everyone: Python</p>
                    <div>
                        <span>17 Lessons</span>
                        <span>62 Students</span>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.container{
    width: 1200px;
    margin: 0 auto;
    padding: 150px 0;
    
    .curiosity-row{
        text-align: center;
        display: flex;
        justify-content: space-around;
        margin-bottom: 150px;
    }

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

            .youtube-logo{
                position: absolute;
                top: -50%;
                left: -50%;
                transform: translate(-50%, -50%);
            }
        }

        .courses-container{
            padding: 30px;
            width: calc(100% / 3);

            img{
                border-radius: 5px 5px 0 0;
                width: 100%;
            }

            .courses-text{
                padding: 30px;
                border-radius: 0 0 5px 5px;
                p{
                    margin: 15px 0 30px;
                    font-weight: bold;
                    font-size: 20px;
                }

                span{
                    margin-right: 30px;
                    color: grey;
                }
            }
        }
    }
}
</style>