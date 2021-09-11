<template>
  <v-main>
    <v-parallax
      dark
      src="https://cdn.vuetifyjs.com/images/backgrounds/vbanner.jpg"
    >
      <v-row align="center" justify="center">
        <v-col class="text-center" cols="12">
          <h1 class="display-1 font-weight-thin mb-4">PORTFOLIO</h1>
          <div id="samplecode">
            <p class="typewritertext typewriteranime">SHIOTA portfolio</p>
          </div>
        </v-col>
      </v-row>
    </v-parallax>
    <v-container class="pb-16">
      <h2 class="headline font-weight-bold text-center my-16">WORKS</h2>
      <section class="section">
        <ProductList></ProductList>
      </section>
      <section class="section">
        <div class="inner">
          <div class="section-title-block">
            <h2 class="headline font-weight-bold text-center my-16">SKILL</h2>
            <skillList></skillList>
          </div>
        </div>
      </section>
      <section class="section">
        <div class="inner">
          <div class="section-title-block">
            <h2 class="headline font-weight-bold text-center my-16">CONTACT</h2>
            <p class="section-desc text-center">
              お問合わせは下記からご連絡をください。
            </p>
          </div>
          <div class="contact-wrapper">
            <div class="contact-list">
              <v-row class="text-center">
                <v-col>
                  <v-btn href="" x-large color="success" dark
                    >Extra large Button</v-btn
                  >
                </v-col>
              </v-row>
            </div>
          </div>
        </div>
      </section>
    </v-container>
  </v-main>
</template>

<script>
import ProductList from "../components/ProductList.vue";
import SkillList from "../components/SkillList.vue";
export default {
  name: "Home",
  components: { ProductList, SkillList },
};
</script>
    <style>
.typewritertext {
  width: 6em;
  margin: 0 auto;
  border-right: 2px solid #37b507;
  font-weight: bold;
  text-align: center;
  white-space: nowrap;
  overflow: hidden;
}

/* Animation */
.typewriteranime {
  animation: typewriter 3s steps(19) 1s 1 normal both,
    blinkCursor 500ms steps(19) infinite normal;
}
@keyframes typewriter {
  from {
    width: 0;
  }
  to {
    width: 7.8em;
  }
}
@keyframes blinkCursor {
  from {
    border-right-color: #37b507;
  }
  to {
    border-right-color: transparent;
  }
}
</style>