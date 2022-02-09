<template>
    <div class="container">
        <learn-about-row />
        <some-data-row />
        <upgrade-skill-row />
        <latest-courses-row />
        <why-people-row />
        <transform-you-row />
        <latest-from-blog-row />
        <subscribe-row />
    </div>
</template>

<script>
import LearnAboutRow from './Row-1-LearnAbout.vue'
import SomeDataRow from './Row-2-Data.vue'
import UpgradeSkillRow from './Row-3-UpgradeSkill.vue'
import LatestCoursesRow from './Row-4-LatestCourses.vue'
import WhyPeopleRow from './Row-5-WhyPeople.vue'
import TransformYouRow from './Row-6-TransformYou.vue'
import LatestFromBlogRow from './Row-7-LatestBlog.vue'
import SubscribeRow from './Row-8-Subscribe.vue'


export default {
    components:{
        UpgradeSkillRow,
        LearnAboutRow,
        LatestCoursesRow,
        WhyPeopleRow,
        TransformYouRow,
        SubscribeRow,
        SomeDataRow,
        LatestFromBlogRow
    },
}
</script>

<style lang="scss" scoped>


.container{
    width: 1200px;
    margin: 0 auto;
    padding: 150px 0;
    
}
</style>