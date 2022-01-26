<template>
    <div class="contact">
        <h2>Contact Us</h2>
        <h4>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Ea doloremque harum dolorum aspernatur reiciendis a, eum reprehenderit accusantium perferendis tempore illo maxime, incidunt recusandae facere quis aliquam doloribus pariatur porro. Molestias ab commodi minus incidunt, earum adipisci rerum ipsa nihil labore rem totam excepturi quibusdam magnam eius atque laborum consequuntur.</h4>
        <div class="leftright">
            <div class="left">
                <span class="tel">Telephone:</span><br>
                <div class="tel1">
                    <span>+998932281884</span><br>
                    <span>+998932281884</span><br>
                    <span>+998906231884</span>
                </div><br>
                <span class="tel">Email:</span><br>
                <span class="tel1">botircoders@gmail.com</span>
            </div>
            <div class="right">
                <span>Subscribe!</span><br>
                <input type="text" placeholder="Name"><br>
                <input type="email" placeholder="Email"><br>
                <input type="password" placeholder="Password"><br>
                <button>submit</button>
            </div>
        </div>
        <footer-menu />
    </div>
</template>
<script>
import FooterMenu from './FooterMenu.vue'
export default {
    components:{
        FooterMenu,
    }
}
</script>
<style scoped>
.contact{
    background-image: url('../assets/img/contact.jpg');
    width: 100%;
    height: 500px;
    background-attachment: fixed;
    background-position: bottom;
    background-size: cover;
}
.contact > h2{
    color: whitesmoke;
    font-size: 50px;
    padding-top: 20px;
    padding-bottom: 20px;
    text-align: center;
}
.contact > h4{
    padding-left: 30px !important;
    padding-right: 30px !important;
    color: white;
    text-align: center;
    font-size: 20px;
    font-style: italic;
}
.contact > .leftright{
    width: 100%;
    border-bottom: black 2px solid;
    height: 260px;
}
.contact > .leftright > .left{
    float: left;
    width: 50%;
    padding-top: 20px;
    padding-bottom: 20px;
    text-align: center;
}
.contact > .leftright > .right{
    float: right;
    width: 50%;
}
.contact > .leftright > .right{
    color: royalblue;
    font-size: 30px;
    padding-top: 20px;
    padding-bottom: 20px;
    text-align: center;
}
.contact > .leftright > .right > input{
    padding: 7px;
    font-size: 20px;
    margin: 5px;
    border-radius: 10px;
    border: coral 1px solid;
}
.contact > .leftright > .right > button{
    border: 1px solid crimson;
    font-size: 25px;
    color: white;
    padding: 10px;
    padding-left: 20px;
    padding-right: 20px;
    background: red;
    border-radius: 10px;
}
.tel{
    color: royalblue;
    font-size: 30px;
}
.tel1{
    color: white;
    font-size: 20px;
}



</style>