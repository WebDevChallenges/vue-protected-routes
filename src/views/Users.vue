<template>
  <div>
    <p>Users</p>
    <button @click=logout>Logout</button>
  </div>
</template>

<script>
import { mapActions } from 'vuex';

export default {
  methods: {
    ...mapActions([
      'logout'
    ])
  },
}
</script>