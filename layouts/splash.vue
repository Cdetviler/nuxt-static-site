<template>
<div>
  <Header />
  <div>
    <div class="bg-overlay">
    </div>
  </div>
  <main class="min-h-screen">
    <nuxt/>
  </main>
</div>
</template>

<script>
import Header from '~/components/Header.vue'

export default {
  components: {
    Header
  }
}
</script>


<style scoped>

  main {
    background-image: url("/daniel-mccullough-1920x1080.jpg");
    background-size: cover;
  }

  .bg-overlay {
    background: linear-gradient(135deg,rgba(17,38,99,0.85) 0%,rgba(44,44,56,0.85) 100%);
    opacity: 0.8;
    display: block;
    position:absolute;
    top: 0px;
    left: 0px;
    z-index: 2;
    width: 100%;
    height: 100%;
  }
</style>
