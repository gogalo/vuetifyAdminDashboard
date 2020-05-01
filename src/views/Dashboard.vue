<template>
  <div class="dashboard">
    <h1>This is an dashboard page</h1>
    <v-btn @click="$router.push('/login')" flat>Login</v-btn>
  </div>
</template>

<script>

export default {
  name: 'Dashboard',
  created () {
    this.$store.commit('SET_LAYOUT', 'base-layout')
  }
}
</script>
