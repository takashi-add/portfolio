<template>
  <div>
    <v-row>
      <product v-for="(product, key) in products" :key="key" :product="product"></product>
    </v-row>
  </div>
</template>
<script>
  import Product from "./Product.vue";
export default {
  name: "ProductList",
  components: {
    Product
  },
  data: () => ({
    products: [{
      id: 1,
      name: "work1",
      image: "../assets/works/dummyimage.png",
      year: "2020",
      category: "コーポレート",
      use: "html css JS",
    }, {
      id: 2,
      name: "work2",
      image: "../assets/works/dummyimage.png",
      year: "2019",
      category: "LP",
      use: "Vue.js",
      info: "",
    }, {
      id: 3,
      name: "work3",
      image: "../assets/works/dummyimage.png",
      year: "2018",
      category: "ECサイト",
      use: "デザイン",
    }, {
      id: 4,
      name: "work4",
      image: "../assets/works/dummyimage.png",
      year: "2019",
      category: "LP",
      use: "Vue.js",
      info: "",
    }, ],
  }),
}; </script>