<template>
  <footer class="text-xs p-4 mt-2">
    <Wrapper>
      © 2019 Charlie Detviler.
    </Wrapper>
  </footer>
</template>

<script>
import Wrapper from '~/components/Wrapper.vue'

export default {
  components: {
    Wrapper
  }
}
</script>

<style>
  footer {
    color: theme('colors.white');
    background-color: theme('colors.grey.dark');
  }
</style>
