<template>
<div>
  <div>
    <HeroText
      text="Charlie Detviler"
      subText="Front End Developer"
      textSize="6xl"
      subTextSize="2xl"
    />
  </div>
</div>
</template>

<script>
import HeroText from '~/components/HeroText.vue';

export default {
  components: {
    HeroText
  },
  layout: 'splash'
}
</script>

<style>

</style>

