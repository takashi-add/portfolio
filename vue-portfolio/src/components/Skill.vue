<template>
  <v-col cols="12" sm="6" md="4" lg="4">
    <v-card class="mx-auto" :href="skills.href">
      <v-img class="white--text align-end" height="200px" :src="skill.image">
      </v-img>
      <v-card-subtitle class="pb-0">{{ skill.year }}</v-card-subtitle>
      <v-card-text class="text--primary">
        <div>{{ skill.category }}</div>
        <div>{{ skill.use }}</div>
        <div>{{ skill.page }}</div>
        <div>{{ skill.tool }}</div>
        <div>{{ skill.info }}</div>
        <div>{{ skill.time }}</div>
      </v-card-text>
    </v-card>
  </v-col>
</template>
          <script>
export default {
  name: "Skill",
  props: ["skill"],
};
</script>