<template>
    <section class="main-content">
        <div class="container">
            <div class="main-content-introduction text-center">

                <MainIntroduction />

                <div class="main-content-posts container">
                    <h4>Featured products</h4>
                    <div class="row">
                        <ProductSingle
                            v-for="product in products"
                            :key="product.id"
                            :product="product"
                        />
                  </div>
                </div>

                <div id="load-more">
                  <a class="btn light load-btn" href="#" role="button">Load more</a>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
import ProductSingle from "@/components/ProductSingle";
import MainIntroduction from "@/components/MainIntroduction";
import products from "@/data/prodcts.json";

export default {
    name: "Body",
    components: {
        ProductSingle,
        MainIntroduction
    },
    data() {
        return {
            row: true,
            products: products
        }
    }
}
</script>

<style scoped>

</style>
