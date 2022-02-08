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
                    <p>facebook</p>
                    <p>facebook</p>
                    <p>facebook</p>
                    <p>facebook</p>
                </div>
            </div>
            <div>
                <h4>Explore</h4>
                <div class="middle-links">
                    <p v-for="(link, i) in exploreLinks" :key="i">{{link}}</p>
                </div>
            </div>
            <div>
                <h4>Information</h4>
                <p v-for="(link, i) in informationLinks" :key="i">{{link}}</p>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
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
    
        .row{
            display: flex;
            justify-content: space-between;
    
            .social-row{
                display: flex;
    
                p{
                    margin-right: 15px;
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
    
            p{
                color: grey;
                margin: 15px 0 0 0;
            }
        }
    }
}
</style>