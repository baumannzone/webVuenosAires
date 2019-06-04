<template>
<header>
  <div class="containerNavBar">
    <Push>
      <ul class="navList">
          <li v-for="item in listNavBar" :key="item.content">
            <a :href="item.href" :target="item.target" :title="item.title">
              {{ item.content }}
            </a>
          </li>
      </ul>
    </Push>
    <div class="containerBrand">
      <h1>
        <a href="/" class="">Vuenos Aires</a>
      </h1>
    </div>
  </div>
</header>
</template>
<script>
import { Push } from "vue-burger-menu";

export default {
  components: {
    Push
  },
  data() {
    return {
      listNavBar: [
        {
          href: "http://meetupjs.com.ar/calendario.html",
          target: "_blank",
          title: "Ver todos los eventos de la comunidad 😎",
          content: "Eventos"
        },
        {
          href: "https://github.com/vuenos-aires/charlas",
          target: "_blank",
          title: "¿Querés dar una charla? 😉",
          content: "Charlas"
        },
        /* {
          href: 'sponsors.html',
          title: 'Los que ponen la tarasca 🙏',
          content: 'Sponsors'
        }, */
        {
          href:
            "https://github.com/vuenos-aires/charlas/blob/master/CONDUCT.md",
          target: "_blank",
          title: "TL;DR: No seas un imbécil",
          content: "Código de Conducta"
        }
      ],
      statusNav: true
    };
  },
  methods: {}
};
</script>

<style lang="scss">
header {
  font-size: 14px;
  h1 {
    a {
      font-weight: bold;
      color: #445b71;
      text-decoration: none;
    }
  }
  .containerNavBar {
    align-items: center;
    display: flex;
    justify-content: space-between;
    margin: 0 auto;
    padding: 1% 2%;
    width: 80vw;
    .bm-burger-button {
      cursor: pointer;
      height: 24px;
      left: 2%;
      position: sticky;
      top: 2%;
      width: 24px;
      .bm-burger-bars {
        background-color: #445b71;
      }
    }
    .bm-item-list > * {
      display: block;
      list-style: none;
      padding: 0 10px;
      a {
        font-size: 1rem;
        font-weight: bold;
        color: #3eb882;
        cursor: pointer;
      }
      a:hover {
        color: #2c825b;
      }
    }
  }
}
</style>
