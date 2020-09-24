<template>
  <section class="container">
    <main>
      <logo />
      <div class="containertext">
        <p>
          <strong>Vuenos Aires</strong>
          es un meetup donde nos enfocamos en aprender, enseñar y difundir todo
          lo que tenga que ver con el ecosistema de
          <a href="https://vuejs.org" target="_blank">
            Vue.js
          </a>
          .
        </p>
        <p>
          Publicamos eventos en
          <a
            href="https://www.meetup.com/vuenos-aires"
            target="_blank"
          >
            Meetup
          </a>
          y usamos
          <a href="http://slack.meetupjs.com.ar" target="_blank">
            Slack
          </a>
          para comunicarnos. Las noticias las posteamos en
          <a href="https://twitter.com/vuenos_aires" target="_blank">
            Twitter
          </a>
          y subimos código a
          <a href="https://github.com/vuenos-aires" target="_blank">
            Github
          </a>
          .
        </p>
      </div>
    </main>
  </section>
</template>

<script>
import logo from "~/components/Logo.vue";

export default {
  components: {
    logo
  }
};
</script>
<style lang="scss" scoped>
.container {
  margin: 0 auto;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  .containertext {
    width: 60%;
    margin: 0 auto;
    font-size: 1.5rem;
    font-weight: 600;
    color: #445b71;
    a {
      color: #3eb882;
      font-weight: 800;
    }
  }
}
@media (max-width: 640px) {
  .container .containertext {
    font-size: 1rem;
    width: 90%;
  }
}
</style>
