<template>
<div>
  <Header />
  <main class="min-h-screen">
    <nuxt/>
  </main>
  <Footer />
</div>
</template>

<script>
import Footer from '~/components/Footer.vue'
import Header from '~/components/Header.vue'

export default {
  components: {
    Footer,
    Header
  }
}
</script>


<style scoped>
  main {
    padding-top: 75px;
  }
</style>

