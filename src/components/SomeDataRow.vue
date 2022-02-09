<template>
    <div class="row">
        <div>
            <h1>129+</h1>
            <p>Enrolled learners</p>
        </div>
        <div>
            <h1>80</h1>
            <p>Finished sessions</p>
        </div>
        <div>
            <h1>4%</h1>
            <p>Satisfaction rate</p>
        </div>
        <div class="bg-absolute-3"></div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
.row{
    text-align: center;
    display: flex;
    justify-content: space-around;
    margin-bottom: 150px;
    position: relative;

    h1{
        color: $montainMeadow;
    }

    .bg-absolute-3{
        position: absolute;
        height: 40px;
        width: 40px;
        bottom: -150px;
        right: 400px;
        border: 5px solid $drifwood;
        border-bottom-color: white;
        border-left-color: white;
        border-radius: 50%;
        transform: rotate(-45deg);
    }
}
</style>