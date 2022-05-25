<template>
  <v-app>
    <v-app-bar
      color="#14213d"
      dark
      shrink-on-scroll
      prominent
      src="https://www.soycest.mx/hs-fs/hubfs/CEST_do%CC%81nde%20puede%20trabajar%20un%20abogado.jpeg?width=744&name=CEST_do%CC%81nde%20puede%20trabajar%20un%20abogado.jpeg"
      fade-img-on-scroll
      scroll-target
      scroll-threshold="1000"
      app
    >
      <template v-slot:img="{ props }">
        <v-img
          v-bind="props"
          gradient="to top right, rgba(0,0,0,.7), rgba(0,0,0,.7)"
        ></v-img>
      </template>

      <v-img
      class="mr-5"
          lazy-src="../src/assets/img/logoBlack.png"
          max-height="100"
          max-width="80"
          src="../src/assets/img/logoWhite.png"
        ></v-img>

      <v-app-bar-title class="te">
      BLOG @Elvis</v-app-bar-title>

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
      <div>
    <v-menu
      v-model="showMenu"
      absolute
      offset-y
    >
    <template v-slot:activator="{ on, attrs }">
        <v-btn icon  v-bind="attrs"
          v-on="on">
        <v-icon>mdi-dots-vertical</v-icon>
      </v-btn>
      </template>
      <v-list>
        <v-list-item
          v-for="(item, index) in items"
          :key="index"
         link exact
        >
         <v-list-item-action>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-action>
          <v-list-item-title>{{ item.title }}</v-list-item-title>
        </v-list-item>
      </v-list>
    </v-menu>
  </div>
      
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
    showMenu: false,
      items: [
        { title: 'Iniciar Sesión',
        icon:'mdi-account'
         },
         { title: 'Detalles',
        icon:'mdi-null'
         },
       
      ],
  }),
};
</script>

<style scoped>
.te{
  color: rgba(255, 255, 255, 0.774);

}
</style>