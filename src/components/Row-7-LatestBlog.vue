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
@import '@/style/variables.scss';
@import '@/style/mainStyle.scss';
.container-fluid{
    width: 100%;
    background-color: $quillGray;

    .container{
        padding: 50px 0;
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
        
            
        }
    }
}
</style>