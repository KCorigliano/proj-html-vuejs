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
import UpgradeSkillRow from './UpgradeSkillRow.vue'
import LearnAboutRow from './LearnAboutRow.vue'
import LatestCoursesRow from './LatestCoursesRow.vue'
import WhyPeopleRow from './WhyPeopleRow.vue'
import TransformYouRow from './TransformYouRow.vue'
import SubscribeRow from './SubscribeRow.vue'
import SomeDataRow from './SomeDataRow.vue'
import LatestFromBlogRow from './LatestFromBlogRow.vue'


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