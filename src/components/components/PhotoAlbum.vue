<template>
    <div class="photoal">
        <img src="../../assets/img/1.jpg" alt="">
        <img src="../../assets/img/2.jpg" alt="">
        <img src="../../assets/img/3.jpg" alt="">
        <img class="x" src="../../assets/img/4.jpg" alt="">
    </div>
</template>
<script>
export default {
    
}
</script>
<style scoped>
.photoal{
    display: flex;
    justify-content: center;
}
.photoal > img{
    border-radius: 50px;
    border: 10px #44444444 solid;
    width: 200px;
    height: 300px;
    margin: 20px;
}
@media (max-width: 700px){
    .photoal{
        width: 89%;
        padding-left: 18px;
    }
    .photoal > img{
        border: 5px;
        width: 100px;
        height: 150px;
        margin: 5px;
    }
    .x{
        display: none;
    }
}
</style>