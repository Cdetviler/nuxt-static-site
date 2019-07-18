<template>
  <div class="hero-text">
    <h1 :class="computedTextSize" class="uppercase text-6xl tracking-wider hero-text-title">{{text}}</h1>
    <h2 :class="computedSubTextSize" class="text-4xl hero-text-subtitle">{{subText}}</h2>
  </div>
</template>

<script>
export default {
  name: 'HeroText',
  props: {
    text: String,
    subText: String,
    textSize: String,
    subTextSize: String
  },
  computed: {
    computedTextSize: function() {
      const result = [];
      if(this.textSize !== null){
        result.push(`text-${this.textSize}`);
      }
      else {
        result.push('text-base');
      }
      return result;
    },
    computedSubTextSize: function() {
      const result = [];
      if(this.subTextSize !== null){
        result.push(`text-${this.subTextSize}`);
      }
      else {
        result.push('text-base');
      }
      return result;
    }
  }
}
</script>

<style scoped>
  .hero-text {
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    color: white;
    text-shadow: 0 0 5px #112663, 0px 0 5px #112663, 0px 0 7px #112663;
    z-index: 5;
    font-weight: 100;
  }

  .hero-text-subtitle {
    font-weight: 300;
  }

  .hero-text-title, .hero-text-subtitle {
    text-align: center;
  }
</style>
