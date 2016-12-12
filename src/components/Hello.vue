<template>
  <div>
    Hi, {{ name }}
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
    console.log(this.$el)
  }
}
</script>
