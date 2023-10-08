<template>
  <Header />

  <main>
    <div class="hero">
      <img
        class="hero__img"
        srcset="
          ./assets/images/image-web-3-desktop.jpg 1600w,
          ./assets/images/image-web-3-mobile.jpg   720w
        "
        src="./assets/images/image-web-3-mobile.jpg"
        alt="Web 3"
      />

      <div class="hero__content">
        <h1 class="hero__title">The Bright Future of Web 3.0?</h1>
        <div>
          <p class="hero__desc">
            We dive into the next evolution of the web that claims to put the
            power of the platforms back into the hands of the people. But is it
            really fulfilling its promise?
          </p>
          <button class="hero__btn">Read more</button>
        </div>
      </div>
    </div>
    <New />
    <Article />
  </main>
</template>

<script>
import Header from "./components/Header.vue";
import New from "./components/New.vue";
import Article from "./components/Articles.vue";
import Footer from "./components/Footer.vue";

export default {
  name: "App",
  components: {
    Header,
    New,
    Article,
    Footer,
  },
};
</script>
