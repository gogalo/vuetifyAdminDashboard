<template>
  <v-app></v-app>
</template>

<script>

export default {
  name: 'Logout',
  created () {
    this.$router.push('/login')
  }
}
</script>