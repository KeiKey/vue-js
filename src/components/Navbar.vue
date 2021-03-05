<template>
  <div>
    <!-- Mobile navbar-->
    <nav class="navbar navbar-expand-lg navbar-dark d-md-none fixed-top mobile-nav">
      <a class="navbar-brand" href="index.html">
        <img src="../assets/img/logo.png" alt="Logo" class="mobile-nav-brand"/>
      </a>
      <a href="#menu-toggle" id="menu-toggle"><span class="navbar-toggler-icon"></span></a>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav">
          <a class="nav-item nav-link" href="index.html">Home</a>
        </div>
      </div>
    </nav>

    <!-- navbar  visible on scroll -->
    <ul class="nav fixed-top justify-content-center scrollable scrollnav" >
      <li class="nav-item">
        <a class="nav-link active" href="index.html">Home</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="contact.html">Contact</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="about.html">About Us</a>
      </li>
      <li class="nav-item">
        <a class="navbar-brand" href="index.html">
          <img src="../assets/img/logo.png" alt="Logo" />
        </a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Locations</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Subscribe</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Shop</a>
      </li>
    </ul>

    <!-- header navbar + brand nav + shop now button -->
    <ul class="nav justify-content-center d-none d-md-flex">
      <li class="nav-item">
        <a class="nav-link active" href="index.html">Home</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="contact.html">Contact</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="about.html">About Us</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Locations</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Subscribe</a>
      </li>
      <li class="nav-item">
        <a class="nav-link" href="#">Shop</a>
      </li>
    </ul>

    <!--    <ul class="nav justify-content-center brand d-none d-md-flex">-->
    <ul class="nav justify-content-center brand">
      <li class="nav-item">
        <a class="navbar-brand" href="index.html">
          <img src="../assets/img/logo.png" alt="Logo" />
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
name: "Navbar"
}
</script>

<style scoped>

.header .nav {
  padding: 30px 0;
}
.header .nav a {
  color: var(--primary-color);
  font-style: normal;
  font-weight: 400;
  font-size: 16px;
  line-height: 20.5px;
  padding: 3px 1px;
  margin: 0 20px;
  text-transform: uppercase;
  letter-spacing: 1px;
}
.header .navbar-brand img {
  height: 125px;
}
.header .navbar-brand img:hover,
.header .nav a:hover,
.header .nav a.active{
  opacity: 0.8;
  transition: opacity 0.3s;
}
.header .scrollable {
  min-height: 95px;
  background-color: var(--secondary-color);
  position: fixed;
  top: 0;
}
.header .scrollable img {
  margin-top: -5px;
  height: 30px;
}

</style>
