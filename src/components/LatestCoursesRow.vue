<template>
<div class="container">
    <h5>JOIN MAXCOACH AT BEST</h5>
    <h1>Latest Online <span>Courses</span></h1>
    <div class="row">
        <div class="courses-container">
            <img src="../assets/images/course-02-480x298.jpg" alt="">
            <div class="courses-text">
                <h2>$40.<span>00</span></h2>
                <p>Learning to Write as a Professional Author</p>
                <div>
                    <span><font-awesome-icon class="icon" icon="file-alt" />20 Lessons</span>
                    <span><font-awesome-icon class="icon" icon="user" />50 Students</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/stock-full-hd-03-480x298.jpg" alt="">
            <div class="courses-text">
                <h2>$0.<span>00</span></h2>
                <p>Curstomer-centric info-Tech Strategies</p>
                <div>
                    <span><font-awesome-icon class="icon" icon="file-alt" />24 Lessons</span>
                    <span><font-awesome-icon class="icon" icon="user" />769 Students</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/stock-full-hd-04-480x298.jpg" alt="">
            <div class="courses-text">
                <h2>$19.<span>00</span></h2>
                <p>Open Programming Courses fro Everyone: Python</p>
                <div>
                    <span><font-awesome-icon class="icon" icon="file-alt" />17 Lessons</span>
                    <span><font-awesome-icon class="icon" icon="user" />62 Students</span>
                </div>
            </div>
        </div>
    </div>
    <div class="radio-row">
        <div class="radio active"></div>
        <div class="radio"></div>
        <div class="radio"></div>
        <div class="radio"></div>
        <div class="radio"></div>
    </div>
    <div class="paragraph">
        <p>Control your personal preference settings to get notified about appropriate courses. <span>View all courses →</span></p>
    </div>
</div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faFileAlt, faUser } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
library.add(faUser);
library.add(faFileAlt);


export default {
    components:{
        FontAwesomeIcon,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
.container{

    h5{
        text-align: center;
        color: $stormDust;
        margin-bottom: 15px;
    }

    h1{
        text-align: center;
        span{
        color: $montainMeadow;
        }
    }
    
    .row{
        display: flex;
        justify-content: space-between;
        align-items: center;
    
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
                margin-top: -5px;

                h2{
                    color: $montainMeadow;

                    span{
                        font-size: 16px;
                        color: $montainMeadow;
                    }
                }

                &:hover{
                    box-shadow: 0 0 10px grey;
                    cursor: pointer;
                    transition: all 0.5s;
                }

                p{
                    margin: 15px 0 30px;
                    font-weight: bold;
                    font-size: 20px;
                }
    
                span{
                    margin-right: 30px;
                    color: grey;

                    .icon{
                        margin-right: 5px;
                    }
                }
            }
        }
    }
    
    .radio-row{
        display: flex;
        justify-content: center;
    
        .radio{
            width: 10px;
            height: 10px;
            color: grey;
            border-radius: 50%;
            margin-right: 15px;
        }
    
        .active{
            width: 15px;
            height: 15px;
            color: black;
        }
    }
    
    .paragraph{
        text-align: center;
        width: 500px;
        margin: 0 auto;
        span{
            cursor: pointer;
            font-weight: bold;
            text-decoration: underline;
        }
    }
}
</style>