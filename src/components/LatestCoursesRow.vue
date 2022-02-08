<template>
<div class="latest-course-container">
    <h1>Latest Online Courses</h1>
    <div class="row">
        <div class="courses-container">
            <img src="../assets/images/course-02-480x298.jpg" alt="">
            <div class="courses-text">
                <h2>$40.00</h2>
                <p>Learning to Write as a Professional Author</p>
                <div>
                    <span>20 Lessons</span>
                    <span>50 Students</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/stock-full-hd-03-480x298.jpg" alt="">
            <div class="courses-text">
                <h2>$0.00</h2>
                <p>Curstomer-centric info-Tech Strategies</p>
                <div>
                    <span>24 Lessons</span>
                    <span>769 Students</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/stock-full-hd-04-480x298.jpg" alt="">
            <div class="courses-text">
                <h2>$19.00</h2>
                <p>Open Programming Courses fro Everyone: Python</p>
                <div>
                    <span>17 Lessons</span>
                    <span>62 Students</span>
                </div>
            </div>
        </div>
    </div>
    <div class="radio-row">
        <div class="radio active"></div>
        <div class="radio"></div>
        <div class="radio"></div>
        <div class="radio"></div>
        <div class="radio"></div>
    </div>
    <div class="paragraph">
        <p>Control your personal preference settings to get notified about appropriate courses. View all courses.</p>
    </div>
</div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
h1{
    text-align: center;
}

.row{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 150px;

    .courses-container{
        padding: 30px;
        width: calc(100% / 3);

        img{
            border-radius: 5px 5px 0 0;
            width: 100%;
        }

        .courses-text{
            padding: 30px;
            border-radius: 0 0 5px 5px;
            p{
                margin: 15px 0 30px;
                font-weight: bold;
                font-size: 20px;
            }

            span{
                margin-right: 30px;
                color: grey;
            }
        }
    }
}
</style>