<template>
  <div :class="[classes, computedAlignment, computedColor, computedTextSize]">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name: 'SectionHeader',
    props: {
      fontSize: {
        type: String,
        default: '4xl'
      },
      color: {
        type: String,
        default: 'primary'
      },
      alignment: {
        type: String,
        default: 'left'
      },
      classes: {
        type: Array,
        default: function () { return [] }
      }
    },
    computed: {
      computedTextSize: function() {
        const result = [];
        result.push(`text-${this.fontSize}`);
        return result;
      },
      computedColor: function() {
        const result = [];
        result.push(`text-color-${this.color}`)
        return result;
      },
      computedAlignment: function() {
        const result = [];
        result.push(`text-${this.alignment}`);
        return result;
      }
    }
  }
</script>

<style scoped>
  .text-color-primary {
    color: theme('colors.grey.black');
  }
  .text-color-secondary {
    color: theme('colors.grey.light');
  }
  .text-color-accent {
    color: theme('colors.accent');
  }
  .text-color-inverted {
    color: theme('colors.white');
  }
</style>