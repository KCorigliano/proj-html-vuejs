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
@import '@/style/row-4-LatestCourses.scss';
</style>