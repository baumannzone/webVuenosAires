<template>
  <img
    src="~/static/vuenosaires_animated.svg"
    alt="Vuenos Aires Meetup"
    class="logo logo-animation"
    title="¡Gracias @camilunghi por el logo! 💪🏼"
  />
</template>
<style lang="scss" scoped>
.logo {
  width: 20%;
}
.logo-animation {
  transition: all 0.25s ease;
}
.logo-animation:hover {
  transform: scale(1.05) translate3d(0, 0, 0);
}
@media (max-width: 640px) {
  .logo {
    width: 50%;
  }
}
</style>
