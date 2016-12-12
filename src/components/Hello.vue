<template>
  <div>
    Hi, {{ name }}
    <p ref="text">Test</p>
  </div>
</template>

<script>
export default {
  props: {
    name: {
      required: true
    }
  },
  beforeCreate () {

  },
  created () {

  },
  mounted () {
    console.log(this.$refs.text)
    $(this.$el)
  },
  beforeUpdate () {
  // change some data and not get infinite loop
  },
  updated () {
  // should not chnage data here it will be infinite loop
  // call jquery
  },
  beforeDestroy () {
  // cleanup listener, callback, subsriber
  },
  destroyed () {

  }
}
</script>
