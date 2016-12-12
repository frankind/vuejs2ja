<template>
  <div>
      <input v-model="name">
      <p v-if="name">Hi, {{ name }}</p>
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