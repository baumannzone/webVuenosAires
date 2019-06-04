<template>
  <footer>
    <div class="containerfooter">
      <div class="containerIcon">
         <a href="https://twitter.com/vuenos_aires" target="_blank"> <fa class="iconFooter" :icon="['fab', 'twitter']" /></a>
        <a href="https://github.com/vuenos-aires" target="_blank"><fa class="iconFooter" :icon="['fab', 'github']" /></a>
      </div>
    </div>
  </footer>
</template>
<script>
export default {
  data() {
    return {};
  },
  methods: {}
};
</script>

<style lang="scss">
footer {
  font-size: 16px;
  border-bottom: 1px solid rgba(0, 0, 0, 0.2);
  h1 {
    a {
      font-weight: bold;
      color: #445b71;
      text-decoration: none;
    }
  }
  .containerfooter {
    align-items: center;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    padding: 1% 2%;
    width: 80vw;
    .containerIcon {
      margin: 0 auto;
      .iconFooter {
        font-size: 2rem;
        color: #445b71;
      }
      .iconFooter:hover {
        font-size: 2rem;
        color: #2c825b;
      }
    }
  }
}
</style>
