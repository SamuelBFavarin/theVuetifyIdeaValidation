<template>
  <v-app id="inspire">
    <v-navigation-drawer
      v-model="drawer"
      app
    >
      <v-list dense>
        
        <v-list-item link>
          <v-list-item-action>
            <v-icon>input</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Home</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-list-item-action>
            <v-icon>contacts</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Usuários</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-list-item-action>
            <v-icon>email</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Access Token</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-list-item-action>
            <v-icon>gesture</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Signature</v-list-item-title>
          </v-list-item-content>
        </v-list-item>

        <v-list-item link>
          <v-list-item-action>
            <v-icon>send</v-icon>
          </v-list-item-action>
          <v-list-item-content>
            <v-list-item-title>Transfer</v-list-item-title>
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
      <v-toolbar-title>Conecta Suite</v-toolbar-title>
    </v-app-bar>

    

    <MenuMain></MenuMain>
     
    
  
  </v-app>
</template>

<script>

  import MenuMain from './MenuMain';

  export default {
    props: {
      source: String,
    },
    components: {
      MenuMain,
    },
    data: () => ({
      drawer: null,
    }),
  }
</script>