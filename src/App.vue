<template>
  <v-app>
    <v-content>
      <v-tabs icons-and-text centered light color="white">
        <v-tab to='/' router>
          Home
          <v-icon>home</v-icon>
        </v-tab>
        <v-tab to='/about' router>
          Search
          <v-icon>search</v-icon>
        </v-tab>
      </v-tabs>
      <router-view/>
    </v-content>
  </v-app>
</template>

<style lang="stylus">
@import '~vuetify/src/stylus/main';

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
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
