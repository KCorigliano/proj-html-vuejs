<template>
    <div class="courses-container">
        <img :src="image" alt="">
        <div class="courses-text">
            <h2>${{price}}.<span>00</span></h2>
            <p>{{title}}</p>
            <div>
                <span><font-awesome-icon class="icon" icon="file-alt" />{{lesson}} Lessons</span>
                <span><font-awesome-icon class="icon" icon="user" />{{student}} Students</span>
            </div>
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
    },
    props:{
        image: String,
        title: String,
        price: Number,
        student: Number,
        lesson: Number,
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/mainStyle.scss';
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
            background-color: white;

            h2{
                color: $montainMeadow;

                span{
                    font-size: 16px;
                    color: $montainMeadow;
                }
            }

            &:hover{
                box-shadow: 0 0 10px $delta;
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
</style>