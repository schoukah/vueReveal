<template>
  <div id="app">
    <div class="reveal">
      <div class="slides">
        <section>
          <div>
            <!-- <img src="./assets/logo.png" /> -->
            <HelloWorld msg="Helloworld works!" />
          </div>
        </section>
        <section>
          <section><H5P /></section>
          <section>Vertical Slide 2</section>
        </section>
      </div>
    </div>
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import Reveal from "reveal.js";
import H5P from "./components/H5P.vue";
// import { render } from "@vue/runtime-dom";

export default {
  name: "app",
  components: {
    HelloWorld,
    H5P,
  },
  mounted() {
    Reveal.initialize();
    // Vue.render((h) => h(H5P));
  },
};
</script>

<style>
@import url("../node_modules/reveal.js/dist/reveal.css");
@import url("../node_modules/reveal.js/dist/theme/white.css");

.reveal {
  height: 100vh;
  overflow: scroll;
}

#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
  height: 100vh;
}
</style>

// slightly adapted from @bricksroo App.vue //
https://gist.github.com/bricksroo/4652f3c37b280e6f977890fb530893de
