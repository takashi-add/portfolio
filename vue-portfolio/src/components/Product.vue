<template>
  <v-col cols="12" sm="6" md="4" lg="4">
    <v-card class="mx-auto" :href="product.href">
      <v-img class="white--text align-end" height="200px" :src="product.image">
        <!--<v-card-title>{{ product.name }}</v-card-title>-->
      </v-img>
      <v-card-subtitle class="pb-0">{{ product.year }}</v-card-subtitle>
      <v-card-text class="text--primary">
        <div>{{ product.category }}</div>
        <div>{{ product.use }}</div>
        <div>{{ product.page }}</div>
        <div>{{ product.tool }}</div>
        <div>{{ product.info }}</div>
        <div>{{ product.time }}</div>
      </v-card-text>
      <v-card-actions>
        <v-btn color="orange" :href="product.href" target="_blank"> url </v-btn>
        <v-btn color="orange" :href="product.href" target="_blank">
          INFO
        </v-btn>
      </v-card-actions>
    </v-card>
  </v-col>
</template>
<script>
export default { name: "Product", props: ["product"] };
// propsを親コンポーネントに送信
</script>
<style></style>