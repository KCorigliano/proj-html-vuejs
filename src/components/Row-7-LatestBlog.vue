<template>
<div class="container">
    <h1>Latest Online Courses</h1>
    <div class="row">
        <div class="courses-container">
            <img src="../assets/images/artist-blog-03-480x325.jpeg" alt="">
            <div class="courses-text">
                <h2>ARTIST</h2>
                <p>Brush Strokes Energize Trees in Paintings</p>
                <div>
                    <span>May 15, 2020</span>
                    <span>688 views</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/artist-blog-01-480x325.jpg" alt="">
            <div class="courses-text">
                <h2>ARTIST</h2>
                <p>Pocket-Sized Notebooks Hold Miniature Paintings</p>
                <div>
                    <span>May 15, 2020</span>
                    <span>603 views</span>
                </div>
            </div>
        </div>
        <div class="courses-container">
            <img src="../assets/images/artist-blog-02-480x325.jpg" alt="">
            <div class="courses-text">
                <h2>ARTIST</h2>
                <p>Connection Between Self-Portraits and Identity</p>
                <div>
                    <span>May 15, 2020</span>
                    <span>397 views</span>
                </div>
            </div>
        </div>
    </div>
</div>
</template>

<script>
export default {
    
}
</script>

<style lang="scss" scoped>
.container{

    h1{
        text-align: center;
    }
    
    .row{
        display: flex;
        justify-content: space-between;
        align-items: center;
    
        .courses-container{
            padding: 30px;
            width: calc(100% / 3);
    
            img{
                border-radius: 5px 5px 0 0;
                width: 100%;
                margin-bottom: 0;
            }
    
            .courses-text{
                padding: 30px;
                border-radius: 0 0 5px 5px;
                margin-top: -5px;

                p{
                    margin: 15px 0 30px;
                    font-weight: bold;
                    font-size: 20px;
                }
    
                span{
                    margin-right: 30px;
                    color: grey;
                    transition: all 0.5s;
                }

                &:hover{
                    box-shadow: 0 0 10px grey;
                    cursor: pointer;
                    transition: all 0.5s;
                }
            }
        }
    }
    
    .radio-row{
        display: flex;
        justify-content: center;
    
        .radio{
            width: 10px;
            height: 10px;
            color: grey;
            border-radius: 50%;
            margin-right: 15px;
        }
    
        .active{
            width: 15px;
            height: 15px;
            color: black;
        }
    }
    
    .paragraph{
        text-align: center;
        width: 500px;
        margin: 0 auto;
    }
}
</style>