<template>
    <div class="courses-container">
        <img :src="image">
        <div class="courses-text">
            <h5>{{role}}</h5>
            <p>{{title}}</p>
            <div>
                <span><font-awesome-icon class="icon" icon="calendar" />{{date}}</span>
                <span><font-awesome-icon class="icon" icon="eye" />{{views}}</span>
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
        FontAwesomeIcon,
    },
    props:{
        image: String,
        title: String,
        role: String,
        date: String,
        views: String,
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/mainStyle.scss';

.courses-container{
    padding: 30px;
    width: calc(100% / 3);

    img{
        border-radius: 5px 5px 0 0;
        width: 100%;
        margin-bottom: 0;
    }

    .courses-text{
        padding: 30px 0;
        border-radius: 0 0 5px 5px;
        margin-top: -5px;

        h5{
            text-align: left;
            margin-bottom: 5px;
            color: $stormDust;
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
    }
}

</style>