<template>
  <div>
    <div class="pt-10 pb-10">
      <div class="d-flex justify-center align-center">
        <v-img
          lazy-src="../assets/img/logoWhite.png"
          max-height="250"
          max-width="350"
          src="../assets/img/logoBlack.png"
        ></v-img>
      </div>
      <div class="d-flex justify-center align-center botones">
        <v-btn-toggle v-model="toggle_exclusive" group>
          <v-btn>
            <v-icon>mdi-facebook</v-icon>
          </v-btn>
          <v-btn>
            <v-icon>mdi-instagram</v-icon>
          </v-btn>
          <v-btn>
            <v-icon>mdi-youtube</v-icon>
          </v-btn>
          <v-btn>
            <v-icon>mdi-github</v-icon>
          </v-btn>
        </v-btn-toggle>
      </div>
    </div>
    <div class="text2 pt-15 pb-15">
      <v-row>
        <v-col class="d-flex justify-end align-center" cols="12" sm="5">
          <img src="../assets/img/barberia.png" width="300" alt="" />
        </v-col>
        <v-col class="d-flex align-center">
          <div>
            <div class="titulo text-h3 pb-3 font-weight-medium">THE MENS SAID</div>
            <div class="subtitulo text-p pl-10 pr-10">
              Ubicada en Miami, Papi Blendzz es su Colorista y Barbero, brindando todo
              tipo de servicios modernos y creativos en peluquería. Orgulloso de ofrecer a
              mis clientes una amplia gama de peinados, tratamientos, looks y productos
              útiles que reflejan su individualidad y gusto personal. ¡Pasa por aquí hoy!
            </div>
            <v-btn class="mt-10" text outlined dark>
              <v-icon>mdi-cellphone</v-icon>
              Contactenos</v-btn
            >
          </div>
        </v-col>
      </v-row>
    </div>
    <servicios />
    <local />
    <contacto />
    <div class=" text2 pt-10 pb-10">
      <div class="d-flex justify-center align-center">
        <v-img
          lazy-src="../assets/img/logoWhite.png"
          max-height="250"
          max-width="350"
          src="../assets/img/logoWhite.png"
        ></v-img>
      </div>
      <div class="d-flex justify-center align-center botones">
        <v-btn-toggle v-model="toggle_exclusive" group>
          <v-btn dark>
            <v-icon>mdi-facebook</v-icon>
          </v-btn>
          <v-btn dark>
            <v-icon>mdi-instagram</v-icon>
          </v-btn>
          <v-btn dark>
            <v-icon>mdi-youtube</v-icon>
          </v-btn>
          <v-btn dark>
            <v-icon>mdi-github</v-icon>
          </v-btn>
        </v-btn-toggle>
      </div>
    </div>
  </div>
</template>
<script>
import servicios from "@/views/servicios";
import local from "@/views/local";
import contacto from "@/views/contacto";
export default {
  components: { servicios, local, contacto },
  data() {
    return {
      toggle_exclusive: undefined,
    };
  },
};
</script>
<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Montserrat:wght@100;200&display=swap");
.img {
  width: 300px;
}
.botones {
  margin-top: -40px;
}
.text2 {
  background: #000;
  color: #f4f4f4;
}
.titulo {
  color: #f0a500;
  font-family: "Bebas Neue", cursive;
}
.subtitulo {
  color: #f4f4f4;
  font-family: "Montserrat", sans-serif;
}
</style>
