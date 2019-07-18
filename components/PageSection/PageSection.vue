<template>
  <section class="pt-10 pb-10" :class="{ 'inverted-section': inverted }">
    <Wrapper>
      <slot></slot>
    </Wrapper>
  </section>
</template>

<script>
  import Wrapper from '~/components/Wrapper.vue'

  export default {
    name: 'PageSection',
    props: {
      inverted: Boolean,
      default: false
    },
    components: {
      Wrapper
    }
  }
</script>

<style scoped>
  .inverted-section {
    background-color: theme('colors.accent');
    color: theme('colors.white');
  }
</style>