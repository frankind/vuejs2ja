<template>
  <div>
      <input v-model="name">
      <p>{{ name }}</p>
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