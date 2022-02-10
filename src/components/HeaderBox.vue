<template>
    <div class="container">
        <div class="links">
            <span v-for="(link, i) in headerLinks" :key="i">
                {{link}}
                <font-awesome-icon class="arrow" icon="chevron-down" />
            </span>
        </div>
        <img :src="headerLogo" alt="">
        <div class="inputs">
            <font-awesome-icon class="icon" icon="shopping-cart" />
            <font-awesome-icon class="icon" icon="user-circle" />
            <input type="text" placeholder="Search...">
        </div>
    </div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faSearch, faShoppingCart, faUserCircle } from '@fortawesome/free-solid-svg-icons'
import { faChevronDown } from '@fortawesome/free-solid-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
library.add(faSearch);
library.add(faChevronDown);
library.add(faShoppingCart);
library.add(faUserCircle);

export default {
    components:{
        FontAwesomeIcon,
    },
    props:{
        headerLinks: Array,
        headerLogo: String
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/headerBox.scss';
</style>