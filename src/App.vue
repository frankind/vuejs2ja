<template>
  <div>
    <input v-model="name">
    <p v-if="name && name !== 'frankind' ">Hi, {{ name }}</p>
    <p v-else-if="name === 'frankind'">:D</p>
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