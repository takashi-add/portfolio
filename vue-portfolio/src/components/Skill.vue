<template>
  <v-col cols="12" sm="6" md="4" lg="4">
    <v-card class="mx-auto" :href="skills.href">
      <v-img class="white--text align-end" height="200px" :src="skills.image">
      </v-img>
      <v-card-subtitle class="pb-0">{{ skills.year }}</v-card-subtitle>
      <v-card-text class="text--primary">
        <div>{{ skills.category }}</div>
        <div>{{ skills.use }}</div>
        <div>{{ skills.page }}</div>
        <div>{{ skills.tool }}</div>
        <div>{{ skills.info }}</div>
        <div>{{ skills.time }}</div>
        <div>aaaa</div>
      </v-card-text>
    </v-card>
  </v-col>
</template>
          <script>
export default {
  name: "Skill",
  props: ["skill"]
};
</script>