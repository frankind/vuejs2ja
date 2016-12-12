<template>
  <div>
    <input v-model="name">
    <p v-if="name">Hi, {{ name }}</p>
    <p v-else>No Data</p>
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