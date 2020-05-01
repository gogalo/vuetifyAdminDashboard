<template>
  <v-card class="elevation-12">
    <v-card-text>
      <v-form>
        <v-text-field
          label="Usuario"
          name="login"
          prepend-icon="mdi-account"
          type="text"
        />

        <v-text-field
          id="password"
          label="Contraseña"
          name="password"
          prepend-icon="mdi-lock"
          type="password"
        />
      </v-form>
    </v-card-text>
    <v-card-actions>
      <v-btn @click="$router.push('/')" flat>
        <v-icon>mdi-view-dashboard</v-icon>
      </v-btn>
      <v-spacer />
      <v-btn
        color="indigo"
        flat
        dark
      >
        Entrar
      </v-btn>
    </v-card-actions>
  </v-card>
</template>

<script>

export default {
  name: 'Login',
  created () {
    this.$store.commit('SET_LAYOUT', 'login-layout')
  }
}
</script>