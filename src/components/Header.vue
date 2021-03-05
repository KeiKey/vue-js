<template>
  <div class="header">
    <Navbar />

    <div id="shop-button">
      <a class="btn dark" href="#" role="button">Shop now</a>
    </div>
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";

export default {
  name: "Header",
  components: {
    Navbar
  }
}
</script>

<style scoped>

.header {
  height: 100vh;
  background-image: url("https://cdn.pixabay.com/photo/2016/09/01/19/53/pocket-watch-1637394_1280.jpg");
  background-size: cover;
}

</style>
