<!-- Archivo principal de Vue para organizar barra de navegación e incluir el contenido como componente (SinglePage) -->

<template>
  <v-app>
    <v-app-bar app dark class="hidden-sm-and-down">
      <v-img src="@/assets/logo_ReDOC.png" max-width="100" contain class=" mr-2" @click="$vuetify.goTo('#inicio', options)" style="cursor: pointer;"></v-img>

      <v-spacer></v-spacer>

      <v-btn text @click="$vuetify.goTo('#redoc', options)">ReDOC</v-btn>
      <v-btn text @click="$vuetify.goTo('#magistrales', options)">Conferencistas</v-btn>
      <v-btn text @click="$vuetify.goTo('#ejes', options)">Líneas</v-btn>
      <v-btn text @click="$vuetify.goTo('#programa', options)">Programa</v-btn>
      <v-btn text @click="$vuetify.goTo('#sala', options)">Proyecciones</v-btn>
      <v-btn text @click="$vuetify.goTo('#inscripcion', options)">Inscripciones</v-btn>
      <v-btn text @click="$vuetify.goTo('#fechas', options)">Fechas</v-btn>
      <v-btn text @click="$vuetify.goTo('#comite', options)">Comité</v-btn>
      <v-btn text @click="$vuetify.goTo('#contacto', options)">Contacto</v-btn>
    </v-app-bar>

    <!-- Carga de asset para fondo de pantalla -->
    <v-content class="pt-0 mt-0" :style="{ 'background-image': 'url(' + require('@/assets/BackgroundEncuentro_2.png') + ')' }">
      <SinglePage/>
    </v-content>
  </v-app>
</template>

<script>
import SinglePage from './components/SinglePage';

export default {
  name: 'App',

  components: {
    SinglePage,
  },

  data: () => ({
    // Configuración adicional para el movimiento de pantalla en menús de navbar
    options: {
      duration: 900,
      offset: 0,
      easing: 'easeInOutCubic',
    },
  }),
};
</script>

<style scoped>
/* Fondo de pantalla fijo */
.v-content {
  background-size: cover !important;
  background-attachment: fixed !important;
  background-repeat: no-repeat !important;
  background-position: center center !important;
}
</style>
