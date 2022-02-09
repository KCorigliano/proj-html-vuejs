<template>
    <div class="container-fluid">
        <img src="../../public/images/home-3-hero-bg.jpg" alt="">
        <div class="text">
            <h2>Commence Business</h2>
            <h1>Distant Mentoring Program</h1>
            <button>Download free guidebook →</button>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
.container-fluid{
    position: relative;
    width: 100%;
    margin: 0 auto;
    img{
        width: 100%;
    }
    .text{
        position: absolute;
        color: white;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;

        h1{
            margin: 25px 0;
            text-transform: uppercase;
            font-size: 50px;
        }

        h2{
            font-size: 30px;
        }

        button{
            color: $montainMeadow;
            padding: 15px 30px;
            border-radius: 5px;
            border: none;
            font-weight: bolder;
            transition: all 0.2s;

            &:hover{
                color: white;
                background-color: $montainMeadow;
                cursor: pointer;
                transition: all 0.2s;
            }
        }
    }
}
</style>