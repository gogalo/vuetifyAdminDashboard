<template>
  <v-app id="inspire">
    
    <v-app-bar
      app
      color="indigo"
      dark
    >
      <v-toolbar-title>Adminfy</v-toolbar-title>
    </v-app-bar>
    
    <v-content>
      <v-container
        class="fill-height"
        fluid
      >
        <v-row
          align="center"
          justify="center"
        >
          <v-col
            cols="12"
            sm="8"
            md="4"
          >
             <router-view/>
             
          </v-col>
        </v-row>
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



