<template>
  <img :class="[computedImagePosition, computedImageRoundness]" :alt="alt" :src="src" />
</template>

<script>
  export default {
    props: {
      src: String,
      isRounded: Boolean,
      alt: String,
      alignment: String
    },
    computed: {
      computedImagePosition: function() {
        const result = [];
        const propExists = this.alignment !== null;
        if(propExists && this.alignment === 'left') {
          result.push('mr-auto')
        }
        else if(propExists && this.alignment === 'right') {
          result.push('ml-auto')
        }
        else if(propExists && this.alignment === 'center') {
          result.push('mx-auto')
        }
        return result;
      },
      computedImageRoundness: function() {
        const result = [];
        if(this.isRounded) {
          result.push('rounded-full');
        }
        return result;
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>