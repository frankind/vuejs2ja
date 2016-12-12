<template>
  <div>
      <input v-model="name">
      <p v-text="name"></p>
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