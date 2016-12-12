<template>
  <div>
    <input v-model="name">
    <hello v-bind:name="name"></hello>
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
        name: '',
        list: [
          1, 2, 3, 4, 5
        ]
      }
    },
    methods: {
      sayHello (value) {
        window.alert('Hi, ' + value)
      }
    }
  }
</script>