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
              <v-col cols="0" sm="2"> </v-col>
              <v-col cols="11" sm="8">
                <div class="subtitulo text-p pl-10 pr-10 font-weight-medium text-center">
                  Todo el mundo quiere verse y sentirse lo mejor posible. Durante muchos
                  años, les he dado a mis clientes la oportunidad de renovar su apariencia
                  y salir sintiéndose bien con mis servicios profesionales de cabello en
                  Miami. Hago de su satisfacción mi objetivo número uno y adapto mis
                  servicios de acuerdo con su solicitud específica. ¡Pase por aquí hoy!
                </div>
              </v-col>
              <v-col cols="0" sm="2"></v-col>
            </v-row>

            <v-btn class="mt-10" text outlined dark>
              <v-icon>mdi-cellphone</v-icon>
              Contactenos</v-btn
            >
          </div>
        </v-col>
      </v-row>
    </div>

    <v-sheet class="mx-auto d-flex justify-center" elevation="8">
      <v-slide-group v-model="model" class="pa-4" show-arrows>
        <v-slide-item v-slot="{ active, toggle }">
          <v-card
            :color="'grey lighten-3'"
            class="ma-4"
            height="500"
            width="400"
            @click="toggle"
          >
            <img
              src="https://elpersonalista.com/wp-content/uploads/2018/04/cortes-cabello-hombres-barba.jpg"
              alt=""
              width="400"
            />
            <v-card-title class="d-flex justify-center text-h5 font-weight-medium titulo"
              >CORTE DE PELO</v-card-title
            >
            <v-card-text class="text-p text-center">
              Quieres estar por encima de los demás y estás deseando que un peluquero
              profesional te peine. Mis servicios de coloración del cabello son únicos y
              le darán a tu cabello el tratamiento y el cuidado de calidad estrella que
              anhelas. ¡Piérdete con un peinado creativo deslumbrante y sal a verte y
              sentirte como una estrella de rock!
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
            class="ma-4"
            height="500"
            width="400"
            @click="toggle"
          >
            <img
              src="https://ath2.unileverservices.com/wp-content/uploads/sites/5/2019/03/cortes-de-pelo-con-barba3.jpg"
              alt=""
              width="400"
            />
            <v-card-title class="d-flex justify-center text-h5 font-weight-medium titulo"
              >ASEO DE HOMBRES</v-card-title
            >
            <v-card-text class="text-p text-center">
              ¿Necesita una nueva apariencia, un estilo fresco o simplemente una limpieza?
              En Papi Blendzz, lo tengo cubierto. Ya sea que tengas el cabello rizado,
              grueso o liso, o una mezcla de algo intermedio, sé cómo ofrecer tu nuevo
              look. Dale a tu cabello la atención que se merece con mis servicios de
              peluquería y disfruta de tu nuevo look.
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
  color: #f0a500;
  font-family: "Bebas Neue", cursive;
}
.subtitulo {
  color: #000000;
  font-family: "Montserrat", sans-serif;
}
</style>
