<template>
    <div class="intro">
        <img src="../../assets/img/intro.jpg" alt="">
        <div class="text">
            <h2>About travels</h2>
            <h3>Lorem ipsum dolor sit amet consectetur adipisicing elit. Aspernatur molestias reiciendis perspiciatis, dolores enim minus voluptatibus dolorum mollitia placeat cum!</h3>
            <h3 class="ip">Lorem ipsum dolor sit amet consectetur, adipisicing elit. Voluptatem saepe in, eaque officia vero modi? Velit atque cumque repellat ex.</h3>
            <a href="#">Photograph</a>
        </div>
    </div>    
</template>
<style scoped>
.intro{
    display: flex;
    justify-content: space-around;
    padding-top: 70px;
    padding-bottom: 70px;
    border-bottom: 2px solid crimson;
}
.intro > img{
    width: 500px;
    border-radius: 10ex;
    border: 10px solid #44444444;
}
.intro > .text{

    display: flex;
    flex-direction: column;
    align-items: center;
    width: 590px;
}
.intro > .text > h2{
    color: royalblue;
    font-size: 50px;
    padding-top: 10px;
    padding-bottom: 15px;
}
.intro > .text > h3{
    color: #444;
    padding: 5px;
    padding-bottom: 8px;
    font-size: 20px;
}
.intro > .text > a{
    border-radius: 50px;
    color: whitesmoke;
    text-decoration: none;
    font-size: 30px;
    margin-top: 10px;
    padding: 20px;
    background-color: royalblue;
}

@media (max-width: 700px) {
    .intro > .text > a{
        border-radius: 50px;
        color: whitesmoke;
        text-decoration: none;
        font-size: 13px;
        margin-top: -10px;
        padding: 10px;
        background-color: royalblue;
    }
    .intro {
        padding-top: 10px;
        padding-bottom: 10px;
        width: 89%;
    }
    .intro > img{
        height: 130px;
        width: 100px;
        border-radius: 10ex;
        border: 5px solid #44444444;
    }
    .ip{
        display: none;
    }
    .intro > .text{
        width: 200px;
    }
    .intro > .text > h2{
        padding: 0 !important;
        font-size: 20px;
        margin: 0 !important;
    }
    .intro > .text > h3{
        padding-left: 5px !important;
        padding: 0 !important;
        font-size: 12px;
    }
}
</style>