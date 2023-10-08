<template>
  <div class="article">
    <div class="article__item" v-for="article in articles" :key="article">
      <img
        class="article__thumbnail"
        :src="article.image.path"
        :alt="article.image.title"
      />
      <div>
        <h3 class="article__number">{{ article.number }}</h3>
        <h4 class="article__title">{{ article.title }}</h4>
        <p class="article__desc">
          {{ article.description }}
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      articles: [
        {
          number: "01",
          title: "Reviving Retro PCs",
          description: "What happens when old PCs are given modern upgrades?",
          image: {
            title: "Retro PC",
            path: require("../assets/images/image-retro-pcs.jpg"),
          },
        },
        {
          number: "02",
          title: "Top 10 Laptops of 2022",
          description: "Our best picks for various needs and budgets.",
          image: {
            title: "Keyboard",
            path: require("../assets/images/image-top-laptops.jpg"),
          },
        },
        {
          number: "03",
          title: "The Growth of Gaming",
          description: "How the pandemic has sparked fresh opportunities.",
          image: {
            title: "Game console",
            path: require("../assets/images/image-gaming-growth.jpg"),
          },
        },
      ],
    };
  },
};
</script>
