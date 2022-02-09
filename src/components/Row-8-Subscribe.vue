<template>
    <div class="sub-container">
        <h1>Subscribe <span>Newsletters</span></h1>
        <p>
            Enter your email address to register to our newsletter subscription
            delivered on a regular basis!
        </p>
        <div>
            <input type="text" placeholder="Enter your email">
            <button>Subscribe</button>
        </div>
        <div class="bg-absolute-1"></div>
        <img class="bg-absolute-2" src="../assets/images/maxcoach-shape-02.png" alt="">
        <img class="bg-absolute-3" src="../assets/images/maxcoach-shape-09.png" alt="">
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/mainStyle.scss';
@import '@/style/variables.scss';

.sub-container{
    text-align: center;
    width: 500px;
    margin: 0 auto;
    position: relative;

    h1{
        margin-bottom: 15px;
        span{
            color: $montainMeadow;
            font-weight: 200;
        }
    }

    .bg-absolute-1{
        position: absolute;
        height: 40px;
        width: 40px;
        top: 100px;
        left: -400px;
        border: 5px solid $montainMeadow;
        border-radius: 50%;
    }

    .bg-absolute-2{
        position: absolute;
        top: 60px;
        right: -300px;
    }

    .bg-absolute-3{
        position: absolute;
        top: -50px;
        right: -310px;
    }
}


button{
    color: white;
    background-color: #1fad95;
    padding: 15px 25px;
    border-radius: 0 5px 5px 0;
    border: none;
    font-weight: bolder;
    transition: all 0.2s;
    margin-top: 50px;
    cursor: pointer;
}
input{
    border-radius: 5px 0 0 5px;
    padding: 15px 25px;
}
</style>