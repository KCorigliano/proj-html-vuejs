<template>
<div class="container-fluid">

    <div class="container">
        <h5>READ FOR MORE JOYMENT</h5>
        <h1>Latest From <span>Our Blogs</span></h1>
        <div class="row">
            <card-box 
                v-for="(card,i) in cards"
                :image="card.image"
                :title="card.title"
                :role="card.role"
                :date="card.date"
                :views="card.views"
                :key="i"
            />
        </div>
    </div>
</div>
</template>

<script>
import CardBox from './BlogsCardBox.vue'

export default {
    components:{
        CardBox
    },
    props:{
        cards: Array,
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/row-7-LatestBlog.scss';
</style>