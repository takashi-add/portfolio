<template>
 <v-main>
   <v-parallax
     dark
     src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
   >
     <v-row align="center" justify="center">
       <v-col class="text-center" cols="12">
         <h1 class="display-1 font-weight-thin mb-4">PORTFOLIO</h1>
         <h4 class="subheading">my portfolio</h4>
       </v-col>
     </v-row>
   </v-parallax>
   <v-container class="pb-16">
     <h2 class="headline font-weight-bold text-center my-16">
       WORKS
     </h2>
     <ProductList></ProductList>
   </v-container>
 </v-main>
</template>
<script>
import ProductList from "../components/ProductList.vue";
export default {
 name: "Home",
 components: { ProductList },
};
</script>