<template>
  <div class="intro">
    <div class="bg-logo">
      <div class="logoNav">
        <logo />
        <div class="nav">
          <a href="#about" class="a">{{ a[0] }}</a>
          <a href="#photo" class="a">{{ a[1] }}</a>
          <a href="#contact" class="a">{{ a[2] }}</a>
        </div>
<!--  -->
        <nav class="navbar">
          <div class="hamburger-menu" v-on:click="menu">
            <div class="line line-1"></div>
            <div class="line line-2"></div>
            <div class="line line-3"></div>
          </div>
          <ul class="nav-list">
            <li class="nav-item">
              <a href="#about" class="nav-link">{{ a[0] }}</a>
            </li>
            <li class="nav-item">
              <a href="#photo" class="nav-link">{{ a[1] }}</a>
            </li>
            <li class="nav-item">
              <a href="#contact" class="nav-link">{{ a[2] }}</a>
            </li>
          </ul>
        </nav>
<!--  -->
      </div>
      <header-text />
    </div>
  </div>
  <about id="about" />
  <photo id="photo" />
  <contact id="contact" />
</template>
<script>
import Logo from "@/components/Logo.vue";
import HeaderText from "@/components/Text.vue";
import About from "@/components/About.vue";
import Photo from "@/components/Photo.vue";
import Contact from "@/components/Contact.vue";
export default {
  components: {
    Logo,
    HeaderText,
    About,
    Photo,
    Contact,
  },
  data() {
    return {
      a: ["About", "Photograph", "Contact"],
    };
  },
  methods: {
    menu(){
      const menuIcon = document.querySelector(".hamburger-menu");
      const navbar = document.querySelector(".navbar");

      menuIcon.addEventListener("click", () => {
        navbar.classList.toggle("change");
      });

    }
  },
};
</script>
<style lang="css">
::-webkit-scrollbar {
  border-radius: 20px;
  border: red 1px solid;
  background: #444;
}
::-webkit-scrollbar-thumb {
  transition: 5s all ease-in;
  border-radius: 20px;
  background: crimson;
  border: coral 1px solid;
}
::-webkit-scrollbar-thumb:hover {
  background: red;
  transition: 5s all ease-out;
}
* {
  margin: 0;
  padding: 0;
}
.body {
  margin: 0;
  padding: 0;
  scroll-behavior: smooth;
  font-family: "Times New Roman", Times, serif;
}
.bg-logo {
  background-image: url("assets/img/bg.jpg");
  background-size: cover;
  background-position: center;
  height: 550px;
  border-bottom: 2px solid crimson;
  border-top: 2px solid crimson;
  background-attachment: fixed;
}
.logoNav {
  width: 100%;
  display: flex;
  justify-content: space-around;
}
.nav {
  width: 560px;
  display: flex;
  justify-content: space-between;
  font-size: 30px;
}
.nav > a {
  text-decoration: none;
  color: white;
  margin-top: 40px;
  height: 50px;
}
.nav > a:hover {
  color: crimson;
  transition: 0.5s all ease-in;
}
nav{
  display: none;
}

.navbar{
  display: none;
}


/*----------------*/
/*      Media     */
/*----------------*/
@media (max-width: 700px) {
 
  #about{
    width: 100%;
    margin: 0 !important;
  }
  .intro{
    width: 100%;
  }
  .bg-logo {
    width: 89%;
    margin: 0 !important;
  }
  #photo{
    width: 89%;
  }
  .nav{
    display: none;
  }
  nav{
    display: inline;
  }
  .navbar{
    display: flex;
  justify-content: center;
  /* align-items: center; */
  padding-top: 100px;
  width: 300px;
  height: 100%;
  background-color: #262626;
  position: fixed;
  top: 0;
  left: -300px;
  border-radius: 0/* 20% 60% 0*/;
  transition: left 0.8s cubic-bezier(1, 0, 0, 1);
  }
  .change{
    left: 0;
  }
  
  .hamburger-menu{
    width: 35px;
    height: 30px;
    position: fixed;
    top: 50px;
    left: 50px;
    cursor: pointer;
    display: flex;
    flex-direction: column;
    justify-content: space-around;
  }
  .line{
    height: 3px;
    background-color: chocolate;
    transition: all 0.8s;
  }
  .change .line-1{
    transform: rotateZ(-405deg) translate(-8px, 6px);
  }
  .change .line-2{
    opacity: 0;
  }
  .change .line-3{
    transform: rotateZ(405deg) translate(-8px, -6px);
  }
  .nav-list{	
    text-align: right;
  }
  .nav-item{
    list-style: none;
    margin: 25px;
  }
  .nav-link{
    text-decoration: none;
    font-size: 22px;
    color: #eee;
    font-weight: 300;
    letter-spacing: 1px;
    text-transform: uppercase;
    position: relative;
    padding: 3px 0;
  }
  .nav-link::before,
  .nav-link::after{
    content: "";
    width: 100%;
    height: 2px;
    background-color: chocolate;
    position: absolute;
    right: 0;
    transform: scaleX(0);
    transition: transform 0.5s;
  }
  .nav-link::after{
    bottom: 0;
    transform-origin: right;
  }
  .nav-link::before{
    top: 0;
    transform-origin: left;
  }
  .nav-link:hover::before,
  .nav-link:hover::after{
    transform: scaleX(1);
  }
}
</style>
