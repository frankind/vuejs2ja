<template>
  <div>
    <input v-model="name">
    <p v-if="name && name !== 'frankind'">Hi, {{ name }}</p>
    <p v-else-if="name === 'frankind'">:D</p>
    <p v-else>No Data</p>
    <button v-on:click="sayHello">Hello</button>
    <p v-for="x in list">{{ x }}</p>
  </div>
</template>

<script>
  export default {
    data () {
      return {
        name: '',
        list: [
          1, 2, 3, 4, 5
        ]
      }
    },
    methods: {
      sayHello () {
        window.alert('Hi, ' + this.name)
      }
    }
  }
</script>