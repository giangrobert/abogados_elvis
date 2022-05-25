<template>
  <div>
    <div class="text2 pt-15 pb-15">
      <v-row>
        <v-col class="d-flex align-center justify-center" cols="12" sm="12">
          <div>
            <div class="titulo text-h2 pb-3 text-center font-weight-medium">
              SERVICIOS
            </div>
            <v-row>
              <v-col cols="0" sm="3"> </v-col>
              <v-col cols="11" sm="6">
                <div class="subtitulo text-p pl-10 pr-10 font-weight-medium text-center">
                  Asesorar y brindar consultorías a personas naturales y jurídicas. Patrocinar y gestionar los intereses de sus clientes. Ser mediador, conciliador o árbitro en asuntos familiares y legales. Negociar y redactar documentos legales (contratos, testamentos, etc).
                </div>
                <div class="d-flex align-center justify-center">
                  <v-btn class="mt-10 mr-2" text outlined>
              <v-icon>mdi-cellphone</v-icon>
              Contactenos</v-btn>
              <v-btn class="mt-10 mr-2" text outlined>
              <v-icon>mdi-cellphone</v-icon>
              Contactenos</v-btn>
              <v-btn class="mt-10 mr-2" text outlined>
              <v-icon>mdi-cellphone</v-icon>
              Contactenos</v-btn>
                </div>
                
              </v-col>
              <v-col cols="0" sm="2">
                
              </v-col>
            </v-row>

            
          </div>
        </v-col>
      </v-row>
    </div>

    <v-sheet class="mx-auto d-flex justify-center col2" elevation="8" c>
      <v-slide-group v-model="model" class="pa-4" show-arrows>
        <v-slide-item v-slot="{ active, toggle }">
          <v-card
            :color="active ? undefined : 'grey lighten-3'"
            class="ma-4 pa-5"
            height="400"
            width="400"
            @click="toggle"
          >
            <img
              src="https://files.lafm.com.co/assets/public/2020-01/abogado.jpg"
              alt=""
              width="360"
            />
            <v-card-title class="d-flex justify-center text-h5 font-weight-medium titulo"
              >DERECHO CORPORATIVO</v-card-title
            >
            <v-card-text class="text-p text-center pr-10 pl-10">
              <a href="">Más información ></a>
            </v-card-text>
            <v-row class="fill-height" align="center" justify="center">
              <v-scale-transition>
                <v-icon
                  v-if="active"
                  color="white"
                  size="48"
                  v-text="'mdi-check'"
                ></v-icon>
              </v-scale-transition>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item v-slot="{ active, toggle }">
          <v-card
            :color="active ? undefined : 'grey lighten-3'"
            class="ma-4 pa-5"
            height="400"
            width="400"
            @click="toggle"
          >
            <img
              src="https://www.soycest.mx/hubfs/carrera-de-abogado.jpeg"
              alt=""
              width="360"
            />
            <v-card-title class="d-flex justify-center text-h5 font-weight-medium titulo"
              >LITIGIOS Y ARBITRAJES</v-card-title
            >
            <v-card-text class="text-p text-center pr-10 pl-10">
              <a href="">Más información ></a>
            </v-card-text>
            <v-row class="fill-height" align="center" justify="center">
              <v-scale-transition>
                <v-icon
                  v-if="active"
                  color="white"
                  size="48"
                  v-text="'mdi-check'"
                ></v-icon>
              </v-scale-transition>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item v-slot="{ active, toggle }">
          <v-card
            :color="active ? undefined : 'grey lighten-3'"
            class="ma-4 pa-5"
            height="400"
            width="400"
            @click="toggle"
          >
            <img
              src="https://guialegal.com/wp-content/uploads/2021/03/contratar-abogado-scaled.jpg"
              alt=""
              width="360"
            />
            <v-card-title class="d-flex justify-center text-h5 font-weight-medium titulo"
              >DERECHO DE SEGUROS</v-card-title
            >
            <v-card-text class="text-p text-center pr-10 pl-10">
              <a href="">Más información ></a>
            </v-card-text>
            <v-row class="fill-height" align="center" justify="center">
              <v-scale-transition>
                <v-icon
                  v-if="active"
                  color="white"
                  size="48"
                  v-text="'mdi-check'"
                ></v-icon>
              </v-scale-transition>
            </v-row>
          </v-card>
        </v-slide-item>
        <v-slide-item v-slot="{ active, toggle }">
          <v-card
            :color="active ? undefined : 'grey lighten-3'"
            class="ma-4 pa-5"
            height="400"
            width="400"
            @click="toggle"
          >
            <img
              src="https://d500.epimg.net/cincodias/imagenes/2019/03/29/legal/1553866445_348039_1553868127_noticia_normal.jpg"
              alt=""
              width="360"
            />
            <v-card-title class="d-flex justify-center text-h5 font-weight-medium titulo"
              >DERECHO ADMINISTRATIVO</v-card-title
            >
            <v-card-text class="text-p text-center pr-10 pl-10">
              <a href="">Más información ></a>
            </v-card-text>
            <v-row class="fill-height" align="center" justify="center">
              <v-scale-transition>
                <v-icon
                  v-if="active"
                  color="white"
                  size="48"
                  v-text="'mdi-check'"
                ></v-icon>
              </v-scale-transition>
            </v-row>
          </v-card>
        </v-slide-item>
      </v-slide-group>
    </v-sheet>
  </div>
</template>
<script>
export default {
  data() {
    return {
      model: null,
    };
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Montserrat:wght@100;200&display=swap");
.img {
  width: 300px;
  margin-left: 500px;
  margin-right: 500px;
}
.botones {
  margin-top: -40px;
}
.text2 {
  background: #f4f4f4;
  color: #000000;
}
.titulo {
  color: #000000;
  font-family: "Bebas Neue", cursive;
}
.subtitulo {
  color: #000000;
  font-family: "Montserrat", sans-serif;
}
.col2{
  background-color: #14213d;
}
</style>
