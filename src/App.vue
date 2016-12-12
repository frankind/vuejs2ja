<template>
  <div>
    <input v-model="name">
    <hello></hello>
  </div>
</template>

<script>
  import Hello from './components/Hello'

  export default {
    components: {
      Hello
    },
    data () {
      return {
        name: ''
      }
    },
    methods: {
      sayHello (value) {
        window.alert('Hi, ' + value)
      }
    }
  }
</script>