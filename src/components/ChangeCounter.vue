<template>
<button @click="increment">Add 1</button>
  <button @click="increase({value: 11})">Add 11</button>

</template>

<script>

import { mapActions } from 'vuex'
export default {
  name: "changeCounter",
  methods: {
    // addOne() {
    //   this.$store.dispatch('increment');
    // }
    ...mapActions(['increment', 'increase'])
  }
}
</script>

<style scoped>

</style>