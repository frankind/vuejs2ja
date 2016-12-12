<template>
  <div>
      <input v-model="name">
      <p v-html="name"></p>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        name: ''
      }
    }
  }
</script>