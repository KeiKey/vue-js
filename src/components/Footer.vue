<template>
  <footer>
    <ContactUs />

    <div class="footer-parent d-none d-md-flex">
      <div class="footer-navigation container">
        <div class="row">
          <div class="col-9">
            <a href="index.html">
              <img src="../assets/img/logo.png" alt="Logo"/>
            </a>
          </div>
          <ul class="footer-links col-3">
            <li class="bold-link">
              <a href="index.html">Cue Shop</a>
            </li>
            <li class="footer-link">
              <a href="index.html" class="active">Home</a>
            </li>
            <li class="footer-link">
              <a href="contact.html">Contact</a>
            </li>
            <li class="footer-link">
              <a href="/about.html">About Us</a>
            </li>
            <li class="footer-link">
              <a href="#">Locations</a>
            </li>
            <li class="footer-link">
              <a href="#">Subscribe</a>
            </li>
            <li class="footer-link">
              <a href="#">Shop</a>
            </li>
          </ul>
        </div>
      </div>
    </div>

    <Copyright />

    <div class="footer-mobile d-md-none">
      <div class="row no-gutters">
        <ul class="nav">
          <li class="nav-item text-center">
            <a class="nav-link active" href="index.html">Home</a>
          </li>
          <li class="nav-item text-center">
            <a class="nav-link" href="contact.html">Contact</a>
          </li>
          <li class="nav-item text-center">
            <a class="nav-link" href="about.html">About Us</a>
          </li>
          <li class="nav-item text-center">
            <a class="nav-link" href="#">Back to top</a>
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<script>
import ContactUs from "@/components/ContactUs";
import Copyright from "@/components/Copyright";
export default {
  name: "Footer",
  components: {
    ContactUs,
    Copyright
  }
}
</script>

<style scoped>
.contact-form {
  background: #fff;
  margin-top: 10%;
  margin-bottom: 5%;
}
.contact-form form {
  padding: 20px;
}
.contact-form form .row {
  margin-bottom: 30px;
}
.contact-form h3 {
  margin-bottom: 8%;
  margin-top: -10%;
  text-align: center;
  color: #000000;
}
.contact-form form .form-control {
  border: 1px solid #000000;
  border-radius: 0;
  height: 60px;
}
.contact-form form textarea {
  height: 210px !important;
}
</style>
