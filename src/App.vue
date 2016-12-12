<template>
  <div>
      <input v-model="name">
      <p v-show="name">Hi, {{ name }}</p>
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