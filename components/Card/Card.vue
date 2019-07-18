<template>
  <div class="mx-auto" :class="computedCardWidth">
    <slot></slot>
  </div>
</template>

<script>
  export default {
    name: 'Card',
    props: {
      width: {
        type: String,
        default: 'md'
      }
    },
    computed: {
      computedCardWidth: function() {
        const result = [];
        result.push(`max-w-${this.width}`);
        return result;
      }
    }
  }
</script>
