<template>
  <v-app>
    <v-app-bar
      color="#cf7500"
      dark
      shrink-on-scroll
      prominent
      src="https://www.beautymarket.es/peluqueria/fotos/12010_not_bmp.jpg"
      fade-img-on-scroll
      scroll-target
      scroll-threshold="500"
      app
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(0,0,0,.7), rgba(0,0,0,.7)"
        ></v-img>
      </template>

      <v-app-bar-nav-icon></v-app-bar-nav-icon>

      <v-app-bar-title>Barbería</v-app-bar-title>

      <v-spacer></v-spacer>

      <v-btn icon to="/">
        <v-icon>mdi-home</v-icon>
      </v-btn>
      <v-btn icon to="/sobremi">
        <v-icon>mdi-account</v-icon>
      </v-btn>
      <v-btn icon to="/videos">
        <v-icon>mdi-movie</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-magnify</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-heart</v-icon>
      </v-btn>

      <v-btn icon>
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
    </v-app-bar>

    <v-main app>
      
      <router-view>
      </router-view>
    </v-main>
  </v-app>
</template>

<script>

export default {
  name: 'App',

  components: {
  },

  data: () => ({
    //
  }),
};
</script>
