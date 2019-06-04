<template>
  <div class="grid-container" id="app">
    <div class="header">
      <navBar />
    </div>
    <div class="container" id="page-wrap">
      <nuxt />
    </div>
    <div class="footer">
      <footers />
    </div>
</div>
</template>
<script>
import navBar from "~/components/navBar.vue";
import footers from "~/components/footer.vue";

export default {
  components: {
    navBar,
    footers
  }
};
</script>
<style>
html {
  font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI",
    Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 18px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}
a {
  text-decoration: none;
}
.grid-container {
  display: grid;
  grid-template-columns: 1fr;
  grid-template-rows: 1fr 100% 1fr;
  grid-template-areas: "header" "container" "footer";
}

.container {
  grid-area: container;
  align-self: center;
}
.header {
  grid-area: header;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
}

.footer {
  grid-area: footer;
  position: absolute;
  bottom: 0px;
  width: 100vw;
}
</style>

