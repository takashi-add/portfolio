<!--<template>
<v-col cols="12" sm="6" md="4" lg="4">
<v-card class="mx-auto">
<v-img class="white--text align-end" height="200px" src="https://dummyimage.com/250x150/000/fff">
<v-card-title></v-card-title>
</v-img>
<v-card-subtitle class="pb-0"></v-card-subtitle>
<v-card-text class="text--primary">
<div></div>
<div></div>
<div></div>
</v-card-text>
<v-card-actions>
<v-btn color="orange" text>LINK </v-btn>
</v-card-actions>
</v-card>
</v-col>
</template>
<script>
  export default {
    name: "Product",
  };
</script>
<style></style>-->

<template>
  <!-- <v-col cols="12" sm="6" md="4" lg="4"> <v-card class="mx-auto"> <v-img class="white--text align-end" height="200px" src="https://dummyimage.com/250x150/000/fff" > <v-card-title></v-card-title> </v-img> <v-card-subtitle class="pb-0"></v-card-subtitle> <v-card-text class="text--primary"> <div></div> <div></div> <div></div> </v-card-text> <v-card-actions> <v-btn color="orange" text> LINK </v-btn> </v-card-actions> </v-card> </v-col> -->
  <div>
    {{ products }}
  </div>
</template>
<script>
export default { name: "Product", props: ["products"] };
</script>
<script>
export default { name: "Product", props: ["products"] };
</script>
<style></style>