<script>
import AppHero from './AppHero.vue'
import AppTitle from './AppTitle.vue'

export default {
  components: {
    AppHero,
    AppTitle
  },
  data() {
    return {
      heroImg: '/Making art-pana.svg',
      heroAlt: 'a girl painting a bird on canvas'
    }
  }
}
</script>


<template>

  <div class="wrapper">

    <div class="d-flex justify-content-between px-5">
      <AppHero class="logo" />
      <nav class="pt-5">
        <ul class="d-flex gap-5 fs-5">
          <li>who we are</li>
          <li>our exhibitions</li>
          <li>our rooms</li>
          <li>contact</li>
        </ul>
      </nav>
    </div>


    <div class="hero">

      <div class="row">
        <div class="col">
          <AppTitle />
        </div>
        <div class="col">
          <img :src="heroImg" :alt="heroAlt">
        </div>
      </div>
    </div>

  </div>
</template>

<style scoped>
.wrapper {
  width: 70%;
  margin: 5vh auto;
  background-color: burlywood;
  border-radius: 30px;
  color: antiquewhite;
}

li {
  list-style-type: none;
  color: black;
  text-transform: uppercase;
  font-weight: 600;
  cursor: pointer;
}

nav {
  height: fit-content;
}

.logo {
  cursor: pointer;
}
</style>