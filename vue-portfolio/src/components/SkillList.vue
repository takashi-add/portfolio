<template>
  <div>
    <v-row>
      <Skill></Skill>
    </v-row>
  </div>
</template>
          <script>
import Skill from "./Skill.vue";
export default {
  name: "SkillList",
  components: { Skill },
  data: () => ({
    skills: [
      {
        id: 1,
        name: "movie create",
        image: "https://htlps.com/portfolio/image/movie-create.jpg",
        year: "2020",
        category: "MOVIE CREATE",
        use: "HTML5/CSS3・JavaScript",
        tool: "制作環境：Visual Studio Code",
        time: "制作時間：1週間",
        page: "ページ構成：1ページ",
        href: "http://htlps.com/portfolio/movie/index.html",
      },
      {
        id: 2,
        name: "cresta design",
        image: "https://htlps.com/portfolio/image/cresta-design.jpg",
        year: "2019",
        category: "CRESTA DESIGN",
        use: "HTML5/CSS3・JQuery・Sass",
        tool: "制作環境：Visual Studio Code",
        time: "制作時間：1週間",
        page: "ページ構成：2ページ",
        href: "http://htlps.com/portfolio/cresta_design/index.html",
      },
      {
        id: 3,
        name: "Shiro",
        image: "https://htlps.com/portfolio/image/shiro.jpg",
        year: "2018",
        category: "SHIRO",
        use: "HTML5/CSS3・JQuery",
        tool: "制作環境：Visual Studio Code",
        time: "制作時間：1週間",
        page: "ページ構成：1ページ",
        href: "http://htlps.com/portfolio/shiro/index.html",
      },
      {
        id: 4,
        name: "きのめ幼稚園",
        image: "https://htlps.com/portfolio/image/kinome.jpg",
        year: "2019",
        category: "きのめ幼稚園",
        use: "HTML5/CSS3・JQuery",
        tool: "制作環境：Visual Studio Code",
        time: "制作時間：1週間",
        page: "ページ構成：2ページ",
        href: "http://htlps.com/portfolio/kinome/index.html",
      },
    ],
  }),
};
</script>