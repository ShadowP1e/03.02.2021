<template>
<v-app id="app">
      <v-navigation-drawer
        color="green"
        dark
        expand-on-hover
        hide-overlay
        permanent
        right
        app>
        <v-list nav 
        shaped
        dense>
        <v-list-item>
          <v-list-item-avatar>
            <v-img src="https://cdn.vuetifyjs.com/images/john.png"></v-img>
          </v-list-item-avatar>
          
          <v-list-item-content class="text-left">
            <v-list-item-title class="font-weight-black">
              SocialLink
            </v-list-item-title>
            <v-list-item-subtitle>Иван Иванов</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
        <v-divider class="my-3"></v-divider>
        <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-home</v-icon>
            </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Главная</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account</v-icon>
            </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Мой профиль</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
        <v-list-item>
            <v-list-item-icon>
              <v-icon>mdi-account-multiple-plus</v-icon>
            </v-list-item-icon>
          <v-list-item-content>
            <v-list-item-title>Найти друзей</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      </v-navigation-drawer>
    
    <v-content class="px-12 py-3">
      <v-container fluid>
        <router-view/>
      </v-container>
    </v-content>

  </v-app>
</template>

<style lang="scss">
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
</style>
