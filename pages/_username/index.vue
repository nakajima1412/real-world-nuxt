<template>
  <div>
    <h1>{{ username }}</h1>
  </div>
</template>

<script>
export default {
  computed: {
    username() {
      return this.$route.params.username
    },
  },
  head() {
    return {
      title: 'User: ' + this.username,
      meta: [
        {
          hid: 'description',
          name: 'description',
          content: 'User Page: ' + this.username,
        },
      ],
    }
  },
}
</script>
