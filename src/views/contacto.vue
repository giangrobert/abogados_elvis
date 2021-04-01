<template>
  <div>
   <v-row class="text2 pt-15 pb-15">
    <v-col cols="0" sm="2"></v-col>
    <v-col cols="12" sm="8">
       <div >
      <div class="titulo text-h2 text-center font-weight-medium pb-5">CONTACTO</div>
      <v-card class="mx-auto" dark>
        <v-card-title>
          <v-icon large left> mdi-account </v-icon>
          <span class="title font-weight-light">Contactarme</span>
        </v-card-title>

        <v-card-text class="pa-10">
          <form>
            <v-text-field :counter="30" label="Nombre" required></v-text-field>
            <v-text-field :counter="30" label="Apellidos" required></v-text-field>
            <v-text-field label="E-mail" required></v-text-field>
            <v-text-field label="Teléfono" required></v-text-field>
            <v-textarea label="Escribenos algo"></v-textarea>
            <v-btn class="mr-4"> Enviar </v-btn>
          </form>
        </v-card-text>

        <v-card-actions>
          <v-list-item class="grow">
            <v-list-item-avatar color="grey darken-3">
              <v-img
                class="elevation-6"
                alt=""
                src="https://avataaars.io/?avatarStyle=Transparent&topType=ShortHairShortCurly&accessoriesType=Prescription02&hairColor=Black&facialHairType=Blank&clotheType=Hoodie&clotheColor=White&eyeType=Default&eyebrowType=DefaultNatural&mouthType=Default&skinColor=Light"
              ></v-img>
            </v-list-item-avatar>

            <v-list-item-content>
              <v-list-item-title>Evan You</v-list-item-title>
            </v-list-item-content>

            <v-row align="center" justify="end">
              <v-icon class="mr-1"> mdi-heart </v-icon>
              <span class="subheading mr-2">256</span>
              <span class="mr-1">·</span>
              <v-icon class="mr-1"> mdi-share-variant </v-icon>
              <span class="subheading">45</span>
            </v-row>
          </v-list-item>
        </v-card-actions>
      </v-card>
    </div>
    </v-col>
    <v-col cols="0" sm="2"></v-col>
   </v-row>
  </div>
</template>
<script>
export default {};
</script>
<style scoped>
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
</style>
