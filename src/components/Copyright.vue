<template>

  <div class="footer-parent footer-copyright d-none d-md-flex">
    <div class="container container-copyright">
      <div class="row">
        <h6 class="col-lg-6 col-md-12">© 2020 ____. All Rights Reserved</h6>
        <h6 class="col-lg-3 col-md-9">Terms and conditions</h6>
        <h6 class="col-lg-3 col-md-3">Website: <a href="#">____</a></h6>
      </div>
    </div>
  </div>

</template>

<script>
export default {
  name: "Copyright"
}
</script>

<style scoped>

.footer-copyright {
  border-top: 0.5px solid var(--tertirary-color);
  height: 15%;
}
.footer-copyright h6 {
  color: #8f8f8f;
}
.footer-copyright h6 a {
  color: var(--primary-color);
  text-decoration: none;
}
.footer-copyright h6 a:hover {
  color: #dedede;
}
.container-copyright {
  padding-top: 20px;
}
.container-copyright h6 {
  font-size: 16px;
}

</style>
