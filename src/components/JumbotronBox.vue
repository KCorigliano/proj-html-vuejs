<template>
    <div class="container">
        <img src="../assets/images/home-3-hero-bg.jpg" alt="">
        <div class="text">
            <h2>Commence Business</h2>
            <h1>Distant Mentoring Program</h1>
            <button>Download free guidebook</button>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.container{
    position: relative;
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
            color: #1fad95;
            padding: 15px 30px;
            border-radius: 5px;
            border: none;
            font-weight: bolder;
            transition: all 0.2s;

            &:hover{
                color: white;
                background-color: #1fad95;
                cursor: pointer;
                transition: all 0.2s;
            }
        }
    }
}
</style>