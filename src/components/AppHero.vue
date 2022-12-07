<script>
export default {
  data() {
    return {
      logo: '/Art-Logo.png',
      logoAlt: 'logo for art & artist'
    }
  }
}
</script>


<template>
  <div class="helloImg">
    <img :src="logo" :alt="logoAlt">
  </div>


</template>

<style scoped>
img {
  max-width: 100%;
}

.helloImg {
  width: 25%;
  height: fit-content;
}
</style>