<template>
    <div class="sub-container">
        <h1>Subscribe Newsletters</h1>
        <p>
            Enter your email address to register to our newsletter subscription
            delivered on a regular basis!
        </p>
        <div>
            <input type="text" placeholder="Enter your email">
            <button>Subscribe</button>
        </div>
    </div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
@import '@/style/mainStyle.scss';
.sub-container{
    text-align: center;
    width: 500px;
    margin: 0 auto;

    h1{
        margin-bottom: 15px;
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