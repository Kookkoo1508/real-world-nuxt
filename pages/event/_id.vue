<template>
  <div>
    <h1>Event# {{ id }}</h1>
  </div>
</template>
<script>
export default {
  computed: {
    id() {
      return this.$route.params.id
    },
  },
  head() {
    return {
      title: 'Event #' + this.id,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'What you need to know about#' + this.id,
        },
      ],
    }
  },
}
</script>
