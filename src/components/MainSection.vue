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

export default {
    name: "Body",
    components: {
        ProductSingle,
        MainIntroduction
    },
    data() {
        return {
            row: true,
            products: [
                {
                    'id':1,
                    'name': "Leather unisex hat" ,
                    'img': "https://cdn.pixabay.com/photo/2020/09/10/18/08/has-5561156_1280.jpg",
                    'alt': "Product image",
                    'tags': [
                        {'id': 1, 'tagName': 'hat'},
                        {'id': 2, 'tagName': 'unisex'},
                        {'id': 3, 'tagName': 'leather'}
                    ]
                },
                {
                    'id':2,
                    'name': "Silver ring",
                    'img': "https://cdn.pixabay.com/photo/2020/10/23/21/58/ring-5680047_1280.jpg",
                    'alt': "Product image",
                    'tags': [
                        {'id': 1, 'tagName': 'ring'},
                        {'id': 2, 'tagName': 'female'},
                        {'id': 3, 'tagName': 'ring'}
                    ]
                },
                {
                    'id':3,
                    'name': "Christmas lights",
                    'img': "https://cdn.pixabay.com/photo/2018/07/10/12/26/lights-3528562_1280.jpg",
                    'alt': "Product image",
                    'tags': [
                        {'id': 1, 'tagName': 'lights'},
                        {'id': 2, 'tagName': 'christmas'}
                    ]
                },
                {
                    'id':4,
                    'name': "Colourful Bracelet",
                    'img': "https://cdn.pixabay.com/photo/2020/09/02/15/09/bracelets-5538539_1280.jpg",
                    'alt': "Product image",
                    'tags': [
                        {'id': 1, 'tagName': 'bracelet'},
                        {'id': 2, 'tagName': 'female'},
                        {'id': 3, 'tagName': 'stainless steel'}
                    ]
                },
                {
                    'id':5,
                    'name': "Omega Speedmaster",
                    'img': "https://cdn.pixabay.com/photo/2020/11/09/15/49/watch-5727064_1280.jpg",
                    'alt': "Product image",
                    'tags': [
                        {'id': 1, 'tagName': 'watch'},
                        {'id': 2, 'tagName': 'omega'},
                        {'id': 3, 'tagName': 'stainless steel'}
                    ]
                },
                {
                    'id':6,
                    'name': "Rope Bracelet",
                    'img': "https://cdn.pixabay.com/photo/2020/08/01/11/53/bracelet-5455220_1280.jpg",
                    'alt': "Product image",
                    'tags': [
                        {'id': 1, 'tagName': 'Bracelet'},
                        {'id': 2, 'tagName': 'gift'},
                        {'id': 3, 'tagName': 'rope'}
                    ]
                }
            ]
        }
    }
}
</script>

<style scoped>

</style>
