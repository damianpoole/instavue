<template>
  <v-app>
    <v-content>
      <v-tabs fixed-tabs>
        <v-tab v-for="n in 3" :key="n">
          Item {{ n }}
          <span class="group pa-2">
            <v-icon>home</v-icon>
          </span>
        </v-tab>
      </v-tabs>
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
