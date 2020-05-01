<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list dense>
        
        <v-list-item 
          @click="$router.push('/')"
          link
          flat
        >
          <v-list-item-action>
            <v-icon>mdi-view-dashboard</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Escritorio</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item 
          @click="$router.push('/list')"
          link
          flat
        >
          <v-list-item-action>
            <v-icon>mdi-pencil-box-multiple</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Listado</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        
        <v-list-item 
          @click="$router.push('/logout')"
          link
          flat
        >
          <v-list-item-action>
            <v-icon>mdi-logout</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Logout</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

      </v-list>
    </v-navigation-drawer>

    <v-app-bar
      app
      color="indigo"
      dark
    >
      <v-app-bar-nav-icon @click.stop="drawer = !drawer" />
      <v-toolbar-title>Adminfy</v-toolbar-title>
    </v-app-bar>

    <v-content>
      <v-container
        fluid
      >
       
       <router-view/>
 
      </v-container>
    </v-content>
    <v-footer
      color="indigo"
      app
    >
      <span class="white--text">&copy; 2020</span>
    </v-footer>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      drawer: null,
    }
  },
  name: 'App'
}
</script>