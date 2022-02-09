<template>
<div class="container">
    <div class="row">
        <div class="text">
            <h4>TESTIMONIALS</h4>
            <h2>Why Do People <span>*Hearts*</span> Us?</h2>
            <p>
                Seeking for verbals of our service quality? Find them here.
                Everything is transparent and straightforward for your sense
                of justification
            </p>
            <p>View all →</p>
        </div>
        <div class="img-box">
            <div class="text-image background">
                <h4>The MaxCoach team works really hard to ensure high level of quality</h4>
                <p>
                    I am happy with their arrangement of lesson and subjects. They
                </p>
                <div class="avatar-row">
                    <img class="avatar" src="../assets/images/testimonial-avata-02.jpg" alt="">
                    <div>
                        <h5>MINA HOLLAGE</h5>
                        <span>/Freelancer</span>
                    </div>
                </div>
            </div>
            <div class="text-image absolute">
                <h4>Professional team of specialist and passionate mentors at reach</h4>
                <p>
                    I need to get a certification for English proficiency and MaxCoach is my best
                    choice. Their tutors are smart and professional when dealing with students
                </p>
                <div class="avatar-row">
                    <img class="avatar" src="../assets/images/testimonial-avata-01.jpg" alt="">
                    <div>
                        <h5>MADLEY PONDOR</h5>
                        <span>/IT Specialist</span>
                    </div>
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
                color: $stormDust;
                margin-bottom: 15px;
                font-weight: 400;
            }
    
            h2{
                font-size: 50px;
                span{
                    color:$montainMeadow;
                    font-weight: 200;
                }
            }
    
            p{
                color: $stormDust;
                line-height: 25px;
                margin-top: 15px;
            }
    
            p:last-child{
                margin-top: 30px;
                color: black;
                font-weight: bold;
                text-decoration: underline;
            }
        }
    
        .img-box{
            width: 60%;
            position: relative;
    
            h4{
                margin: 5px 0;
                line-height: 30px;
            }
    
            p{
                line-height: 30px;
            }
    
            .text-image{
                box-shadow: 0 0 50px $delta;
                border-radius: 5px;
                padding: 25px;
            }
    
            .avatar-row{
                display: flex;
                margin-top: 50px;
                align-items: center;
    
                .avatar{
                    width: 50px;
                    border-radius: 50%;
                    margin-right: 15px;
                }
    
                span{
                    font-size: 12px;
                    color: $delta;
                }
            }
    
        }
    
        .background{
            width: 500px;
            margin: 0 auto;
            filter: opacity(40%);
    
            .avatar-row{
                margin-top: 250px;
            }
        }
    
        .absolute{
            position: absolute;
            background-color: white;
            top: 55%;
            left: 50%;
            transform: translate(-50%, -50%);
            width: 600px;
        }
    }
}

</style>