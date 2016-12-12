<template>
  <div>
    <input v-model="name">
    <hello-component :name="name"></hello-component>
  </div>
</template>

<script>
  import HelloComponent from './components/Hello'

  export default {
    components: {
      HelloComponent
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