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
@import '@/style/blogsCardBox.scss';
</style>