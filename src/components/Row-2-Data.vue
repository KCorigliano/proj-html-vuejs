<template>
<div class="container">
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
        <div class="bg-absolute"></div>
    </div>
</div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
@import '@/style/mainStyle.scss';
.row{
    text-align: center;
    display: flex;
    justify-content: space-around;
    margin-bottom: 150px;
    position: relative;

    h1{
        color: $montainMeadow;
    }

    .bg-absolute{
        position: absolute;
        height: 40px;
        width: 40px;
        bottom: -150px;
        right: 400px;
        border: 5px solid $drifwood;
        border-bottom-color: $quillGray;
        border-left-color: $quillGray;
        border-radius: 50%;
        transform: rotate(-45deg);
    }
}
</style>