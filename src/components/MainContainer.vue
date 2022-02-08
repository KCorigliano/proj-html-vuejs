<template>
    <div class="container">
        <learn-about-row />
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
        <upgrade-skill-row />
        <latest-courses-row />
        <why-people-row />
        <transform-you-row />
        <latest-courses-row />
        <subscribe-row />
    </div>
</template>

<script>
import UpgradeSkillRow from './UpgradeSkillRow.vue'
import LearnAboutRow from './LearnAboutRow.vue'
import LatestCoursesRow from './LatestCoursesRow.vue'
import WhyPeopleRow from './WhyPeopleRow.vue'
import TransformYouRow from './TransformYouRow.vue'
import SubscribeRow from './SubscribeRow.vue'

export default {
    components:{
        UpgradeSkillRow,
        LearnAboutRow,
        LatestCoursesRow,
        WhyPeopleRow,
        TransformYouRow,
        SubscribeRow
    },
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
}
</style>