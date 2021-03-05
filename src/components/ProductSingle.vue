<template>
    <div class="col-lg-6 col-md-12 post">
        <a href="#">
            <img
                class="img-fluid"
                :src="product.img"
                :alt="product.alt"
            />
        </a>
        <h4>
            <span
                v-for="tag in product.tags"
                :key="tag.id"
            >
            {{ tag.tagName }},
            </span>
        </h4>
        <h3>{{ product.name }}</h3>
    </div>
</template>

<script>
export default {
  name: "ProductSingle",
  props: {
    product: {
      type: Object
    }
  }
}
</script>

<style scoped>

.main-content-posts h4 {
  line-height: 20.5px;
  padding: 20px 0 15px 0;
}
.main-content-posts .img-fluid {
  border: 2px solid var(--primary-color);
}
.main-content-posts .img-fluid:hover {
  border: 0;
}
.main-content-posts a:hover {
  opacity: 0.8;
  transition: opacity 0.3s;
}

</style>
