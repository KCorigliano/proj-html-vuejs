<template>
    <div class="courses-container">
        <img :src="image" alt="">
        <div class="courses-text">
            <h2>${{price}}.<span>00</span></h2>
            <p>{{title}}</p>
            <div>
                <span><font-awesome-icon class="icon" icon="file-alt" />{{lesson}} Lessons</span>
                <span><font-awesome-icon class="icon" icon="user" />{{student}} Students</span>
            </div>
        </div>
    </div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faFileAlt, faUser } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
library.add(faUser);
library.add(faFileAlt);
export default {
    components:{
        FontAwesomeIcon,
    },
    props:{
        image: String,
        title: String,
        price: Number,
        student: Number,
        lesson: Number,
    },
}
</script>

<style lang="scss" scoped>
@import '@/style/coursesCardBox.scss';
</style>