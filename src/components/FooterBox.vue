<template>
<div class="container-fluid">
    <div class="container">
        <div class="row">
            <div class="contacts">
                <h4>Address</h4>
                <p>328 NE 191 St # 87394 Miami, FL 33179-3899</p>
                <p>+1 (305) 547-9909 (9am -5 am EST, Monday - Fryday)</p>
                <p>support@maxcoach.com</p>
                <div class="social-row">
                    <p><font-awesome-icon class="icon" :icon="['fab', 'facebook-square']" @click="searchInputShow" /></p>
                    <p><font-awesome-icon class="icon" :icon="['fab', 'twitter']" @click="searchInputShow" /></p>
                    <p><font-awesome-icon class="icon" :icon="['fab', 'instagram']" @click="searchInputShow" /></p>
                    <p><font-awesome-icon class="icon" :icon="['fab', 'linkedin']" @click="searchInputShow" /></p>
                </div>
            </div>
            <div>
                <h4>Explore</h4>
                <div class="middle-links">
                    <p v-for="(link, i) in exploreLinks" :key="i">{{link}}</p>
                </div>
            </div>
            <div class="right-links">
                <h4>Information</h4>
                <p v-for="(link, i) in informationLinks" :key="i">{{link}}</p>
            </div>
        </div>
        <div class="rights-explication">
            <p>©2020 Maxcoach- All Rights Reserved</p>
        </div>
    </div>
</div>
</template>

<script>
import { library } from '@fortawesome/fontawesome-svg-core'
import { faFacebookSquare, faInstagram, faLinkedin, faTwitter } from '@fortawesome/free-brands-svg-icons'
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome'
library.add(faFacebookSquare);
library.add(faInstagram);
library.add(faTwitter);
library.add(faLinkedin);

export default {
    components:{
        FontAwesomeIcon
    },
    props:{
        exploreLinks: Array,
        informationLinks: Array,
    }
}
</script>

<style lang="scss" scoped>

.container-fluid{
    width: 100%;
    background-color: #141423;
    color: white;
    padding: 50px 0;

    .container{
        width: 1200px;
        margin: 0 auto;

        p{
            color: grey;
            margin: 15px 0 0 0;
        }
    
        .row{
            display: flex;
            justify-content: space-between;

            .contacts{

                .social-row{
                    display: flex;
                    color: grey;
                    justify-content: space-between;
                    width: 150px;
                    margin-top: 30px;
                    font-size: 20px;
                }
            }
    
    
            .middle-links{
                display: flex;
                flex-direction: column;
                flex-wrap: wrap;
                height: 100px;
                p{
                    margin: 15px 50px 0 0;
                    cursor: pointer;
                }
            }

            .right-links{
                
                p{
                    cursor: pointer;
                }
            }
    
        }

        .rights-explication{
            text-align: center;
            margin-top: 100px;
        }
    }
}
</style>