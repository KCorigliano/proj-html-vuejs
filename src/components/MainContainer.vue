<template>
<div class="container-fluid">
    <div class="background">
        <div class="background-height"></div>
        <svg class="svg-img" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100" preserveAspectRatio="none" height="100" fill="white"><path class="elementor-shape-fill" d="M0 0v100h100V0Q50 200 0 0"/></svg>
    </div>
    <learn-about-row />
    <some-data-row />
    <upgrade-skill-row />
    <latest-courses-row 
        :cards="coursesCards"
    />
    <why-people-row />
    <transform-you-row />
    <latest-from-blog-row 
        :cards="blogsCards"
    />
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
    props:{
        coursesCards: Array,
        blogsCards: Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
.container-fluid{
    width: 100%;

    .background{
        width: 100%;
        position: absolute;
        z-index: -1;

        .background-height{
            height: 2100px;
            background-color: $quillGray;
        }

        .svg-img{
            width: 100%;
            margin: 0 auto;
            background-color: $quillGray;
        }
    }

}
</style>