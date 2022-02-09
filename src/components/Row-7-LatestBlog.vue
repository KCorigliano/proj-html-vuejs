<template>
<div class="container">
    <h5>READ FOR MORE JOYMENT</h5>
    <h1>Latest From <span>Our Blogs</span></h1>
    <div class="row">
        <div class="courses-container">
            <img src="../assets/images/artist-blog-03-480x325.jpeg" alt="">
            <div class="courses-text">
                <h5>ARTIST</h5>
                <p>Brush Strokes Energize Trees in Paintings</p>
                <div>
                    <span><font-awesome-icon class="icon" icon="calendar" />May 15, 2020</span>
                    <span><font-awesome-icon class="icon" icon="eye" />688 views</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/artist-blog-01-480x325.jpg" alt="">
            <div class="courses-text">
                <h5>ARTIST</h5>
                <p>Pocket-Sized Notebooks Hold Miniature Paintings</p>
                <div>
                    <span><font-awesome-icon class="icon" icon="calendar" />May 15, 2020</span>
                    <span><font-awesome-icon class="icon" icon="eye" />603 views</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/artist-blog-02-480x325.jpg" alt="">
            <div class="courses-text">
                <h5>ARTIST</h5>
                <p>Connection Between Self-Portraits and Identity</p>
                <div>
                    <span><font-awesome-icon class="icon" icon="calendar" />May 15, 2020</span>
                    <span><font-awesome-icon class="icon" icon="eye" />397 views</span>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faCalendar, faEye } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
library.add(faCalendar);
library.add(faEye);

export default {
    components:{
        FontAwesomeIcon
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
.container{

    h5{
        text-align: center;
        color: $delta;
        margin-bottom: 25px;
        font-weight: 400;
    }

    h1{
        text-align: center;
        span{
            color: $montainMeadow;
            font-weight: 200;
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
                margin-bottom: 0;
            }
    
            .courses-text{
                padding: 30px;
                border-radius: 0 0 5px 5px;
                margin-top: -5px;

                h5{
                    text-align: left;
                    margin-bottom: 5px;
                }

                p{
                    margin: 15px 0 30px;
                    font-weight: bold;
                    font-size: 20px;
                }
    
                span{
                    margin-right: 30px;
                    color: $delta;
                    transition: all 0.5s;
                    .icon{
                        margin-right: 5px;
                    }
                }

                &:hover{
                    box-shadow: 0 0 10px $delta;
                    cursor: pointer;
                    transition: all 0.5s;
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
    }
}
</style>