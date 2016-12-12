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
  mounted () {
    console.log(this.$refs.text)
  }
}
</script>
