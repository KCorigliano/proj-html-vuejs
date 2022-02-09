<template>
    <div class="container">
        <h5>JOIN MAXCOACH AT BEST</h5>
        <h1>Latest Online <span>Courses</span></h1>
        <div class="row">
            <card-box 
                v-for="(card,i) in cards"
                :image="card.image"
                :title="card.title"
                :price="card.price"
                :student="card.students"
                :lesson="card.lessons"
                :key="i"
            />
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
import CardBox from './CoursesCardBox.vue'



export default {
    components:{
        CardBox,
    },
    props:{
        cards: Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/mainStyle.scss';
.container{
    padding-top: 50px;

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
    }
    
    .radio-row{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-bottom: 50px;
    
        .radio{
            width: 10px;
            height: 10px;
            background-color: $delta;
            border-radius: 50%;
            margin-right: 15px;
        }
    
        .active{
            width: 15px;
            height: 15px;
            background-color: black;
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