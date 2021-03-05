<template>
  <div id="app">
    <div id="wrapper">
      <Header />

      <MainSection />

      <Footer />
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import MainSection from "@/components/MainSection";

export default {
  name: 'App',
  components: {
      Header,
      Footer,
      MainSection
  }
}
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Open+Sans:wght@300;700&display=swap");
:root {
  --primary-color: #ffffff;
  --secondary-color: #000000;
  --tertirary-color:#5f5f5f;
}
body {
  font-family: "Open Sans", sans-serif;
  overflow-x: hidden;
}
.footer-contact-us {
  border-top: 1px solid var(--tertirary-color);
}
.footer-contact-us .content {
  margin: 40px 0;
}
.footer-contact-us .content .social-icons {
  padding: 15px 0;
  margin-top: 10px;
}
.footer-contact-us .content .social-icons li {
  display: inline-block;
  margin: 0 6px;
  border: 1px solid var(--tertirary-color);
}
.footer-contact-us .content .social-icons i {
  color: var(--secondary-color);
  padding: 0 !important;
  transition: 0.3s;
}
.footer-contact-us .content .social-icons i:hover {
  color: var(--primary-color);
}
.footer-contact-us .content .social-icons .nav-link {
  padding: 4px 9px;
  transition: 0.3s;
}
.footer-contact-us .content .social-icons .nav-link:hover {
  background-color: var(--secondary-color);
}
.footer-contact-us .content h4 {
  padding: 20px 0 15px;
  text-transform: uppercase;
  font-weight: 400;
  font-size: 16px;
}
.footer-contact-us .content input {
  border: 1px solid var(--tertirary-color);
  padding: 3px 6px;
  margin: 10px 0;
  width: 25%;
}
.footer-contact-us .content input::placeholder {
  font-size: 15px;
}
.footer-parent {
  background-color: var(--secondary-color);
}
.footer-navigation {
  padding: 40px 0;
}
.footer-navigation img {
  height: 75px;
}
.footer-links {
  list-style-type: none;
  margin-bottom: 10px;
  line-height: 100%;
}
.footer-link a {
  text-decoration: none;
  color: #8f8f8f;
  line-height: 19px;
  font-weight: 400 !important;
  font-style: normal;
}
.footer-link a:hover {
  color: #bfbfbf;
}
.bold-link a {
  font-weight: 500;
  color: var(--primary-color);
}
.main-content {
  padding-top: 10px;
}
.btn {
  padding: 16px 0;
  text-transform: uppercase;
  min-width: 250px;
  color: var(--primary-color);
  border: 1px solid var(--primary-color);
  border-radius: 0;
}
.btn:hover {
  color: var(--primary-color);
  opacity: 0.5;
  transition: opacity 0.3s;
}
#shop-button {
  position: absolute;
  bottom: 70px;
  margin-left: -124px;
  left: 50%;
}
#load-more {
  margin: 40px 40px 15px 40px;
}
#load-more .load-btn {
  color: var(--secondary-color);
  border-color: var(--secondary-color);
}
.post {
  margin: 30px 0;
}
.show-nav {
  visibility: visible;
}
.hide-nav {
  visibility: hidden;
}
.mobile-nav{
  background-color: transparent;
  min-height: 71px;
}
.mobile-nav .navbar-brand{
  margin-left: -98px;
  padding-left: 50%;
}
.mobile-nav-brand{
  max-height: 45px;
}
.scrollnav{
  display: none;
}
.display-flex{
  display: flex !important;
}
.dark-background{
  background-color: var(--secondary-color) !important;
}
@media (max-width: 992px) {
  .main-content-introduction h3 {
    min-width: 80%;
    margin-left: 10%;
    font-size: 26px;
  }
}
@media (max-width: 768px) {
  .container{
    max-width: 100%;
  }
  .scrollnav{
    display: none !important;
  }
  .main-content-introduction h3 {
    min-width: 90%;
    margin-left: 5%;
  }
  .side-menu {
    height: 300px;
    margin-top: -150px;
    top: 50%;
    position: relative;
  }
  .footer-mobile .nav,
  .side-menu .nav {
    display: inline-block;
    min-width: 100%;
    background-color: var(--secondary-color);
  }
  .footer-mobile .nav .nav-item:hover,
  .side-menu .nav .nav-item:hover {
    background-color: #3C3735;
    opacity:0.9;
  }
  .footer-mobile .nav .nav-item a {
    text-transform: uppercase;
    font-weight: 500;
    line-height: 20.5px;
    color: var(--primary-color);
    padding: 20px 0;
    border-bottom: 1px solid var(--tertirary-color);
  }
  .side-menu .nav .nav-item a {
    text-transform: uppercase;
    font-weight: 400;
    line-height: 27px;
    font-size: 20px;
    color: var(--primary-color);
    padding: 15px 0;
    letter-spacing: 1px;
  }
  .footer-contact-us .content input{
    width: 80%;
  }
  #load-more .load-btn {
    width: 100%;
  }
  .brand .nav-item .navbar-brand img {
    margin-top: 25%;
  }
  #wrapper {
    width: 100vw;
    padding-right: 0;
    transition: all 0.3s ease;
  }
  #wrapper.toggled {
    padding-right: 250px;
  }
  #right-content {
    z-index: 1000;
    position: fixed;
    right: 250px;
    width: 0;
    height: 100%;
    margin-right: -250px;
    transition: all 0.3s ease;
    background-color:#000000;
  }
  #wrapper.toggled #right-content {
    width: 80%;
  }
  #left-content {
    width: 100vw;
    transition: all 0.3s ease;
  }
  #wrapper.toggled #left-content {
    left: 100%;
    margin-left: calc(-199px - 80%);
    transition: all 0.3s ease;
  }
}
@media (max-width: 500px) {
  .header .nav-item .navbar-brand img {
    height: 70px;
    margin-top: 40%;
  }
  .main-content-introduction h3{
    font-size: 20px;
  }
  .post{
    margin: 15px 0;
  }
  .main-content-posts h4{
    padding: 10px 0 0 0;
  }
}

</style>
