<template>
  <div>
    <h1>Events</h1>
    <input v-model="username" type="text" />
    <nuxt-link :to="{ name: 'username', params: { username } }">
      user page
    </nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      username: 'nanashi',
    }
  },
  head() {
    return {
      title: 'Event Listing',
      meta: [
        {
          hid: 'description',
          name: 'description',
          content:
            'Where you can find all the envents taking place in your neighborhood',
        },
      ],
    }
  },
}
</script>
