<template>
  <div>
    <ProductHeader @sortYearChange="sortYearChanged($event)"></ProductHeader>
    <v-row>
      <product
        v-for="(product, key) in filterdList"
        :key="key"
        :product="product"
      >
      </product
    ></v-row>
  </div>
</template>

<script>
import ProductHeader from "./ProductHeader.vue";
// ProductHeader.vueからProductHeader読み込み
import Product from "./Product.vue";
// Product.vueからProductを読み込み
export default {
  name: "ProductList",
  components: { ProductHeader, Product },
  // コンポーネントProductHeader Productを送信
  data: () => ({
    sortYear: "全て",
    products: [
      // 子コンポーネントからpropsを取得
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
  computed: {
    filterdList: function () {
      const newList = [];
      for (let i = 0; i < this.products.length; i++) {
        if (this.sortYear === "2020" && this.products[i].year === "2020") {
          newList.push(this.products[i]);
        } else if (
          this.sortYear === "2019" &&
          this.products[i].year === "2019"
        ) {
          newList.push(this.products[i]);
        } else if (
          this.sortYear === "2018" &&
          this.products[i].year === "2018"
        ) {
          newList.push(this.products[i]);
        } else if (this.sortYear === "全て") {
          newList.push(this.products[i]);
        }
      }
      return newList;
    },
  },
  methods: {
    sortYearChanged: function (year) {
      console.log(year);
      this.sortYear = year;
    },
  },
};
</script>