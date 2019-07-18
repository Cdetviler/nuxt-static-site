<template>
  <ul class="list-disc">
    <li
      class="ml-5 mb-3"
      v-for="listItem in listItems"
      :key="listItem"
    >
      {{listItem}}
    </li>
  </ul>
</template>

<script>
  export default {
    name: 'CardList',
    props: {
      listItems: {
        type: Array,
        default: function () { return [] }
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>