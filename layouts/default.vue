<template>
  <v-app>
    
    <v-navigation-drawer app temporary v-model="drawer" class="grey lighten-5 elevation-6">
      <v-list>
        <v-list-tile v-for="(item, i) in items" :key="i" :to="item.to" router exact :disabled="item.disabled">
          <v-list-tile-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-tile-action>
          <v-list-tile-content>
            <v-list-tile-title v-text="item.title"/>
          </v-list-tile-content>
        </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    
    <v-toolbar clipped-left color="blue" dark fixed app>  
      <v-toolbar-side-icon @click="drawer = !drawer" class="white--text"></v-toolbar-side-icon>
      <v-toolbar-title>Teseu Web</v-toolbar-title>
    </v-toolbar>
    
    <v-content>
      <nuxt/>
    </v-content>
    
    <v-footer absolute color="grey lighten-4">
      <span class="pl-3">&copy; 2019 - <strong>Teseu</strong></span>
    </v-footer>

  </v-app>
</template>

<script>
export default {
  data() {
    return {
      drawer: false,

      items: [
        { icon: 'home', title: 'Início', to: '/', disabled: false },
        { icon: 'map', title: 'Mapa', to: '/map', disabled: true },
        { icon: 'widgets', title: 'Documentação da API', to: '/api-docs', disabled: false },
        { icon: 'vpn_key', title: 'Token da API', to: '/api-token', disabled: false },
        { icon: 'archive', title: 'Exportação de CSV', to: '/csv-export', disabled: true },
        { icon: 'description', title: 'Termos de Uso', to: '/terms-of-use', disabled: false }
      ]
    }
  }
}
</script>
