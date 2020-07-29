<template>
  <v-container pa-0 grid-list-xl fluid>
    <v-layout wrap>
      <v-flex v-for="(item, i) in items" :key="i" xs12 sm6 md4 d-flex child-flex>
        <v-card
          :to="item.to"
          hover
          
        >
          <v-card-title class="title pb-0 align-center">
            <span v-text="item.title"  style="word-break: break-word;"/>
            <template v-if="item.icon">
              <v-spacer />
              <v-icon size="28" v-text="icon" />
            </template>
          </v-card-title>
          <v-card-text class="grey--text text--darken-1" v-text="item.text" />
        </v-card>
      </v-flex>
    </v-layout>
  </v-container>
</template>

<script>
import Logo from "~/components/Logo.vue";
import VuetifyLogo from "~/components/VuetifyLogo.vue";

export default {
  data() {
    return {
      items: [
        {
          title: "LECTURA 1",
          text: "BARROS Y ESPINILLAS",
          to: "matematicas",
        },
        {
          title: "LECTURA 2",
          text: "ASÍ LUCE SINALOA TRAS LA INUNDACIÓN",
          to: "matematicas",
        },
        {
          title: "LECTURA 3",
          text: "Árboles petrificados",
          to: "matematicas",
        },
        {
          title: "LECTURA 4",
          text: "poema",
          to: "matematicas",
        },
        {
          title: "LECTURA 5",
          text: "",
          to: "matematicas",
        },
        {
          title: "LECTURA 6",
          text: "DESALOJAN A CAMPESINOS EN CHIAPAS",
          to: "matematicas",
        },
        {
          title: "LECTURA 7",
          text: "El drama del desencantado",
          to: "matematicas",
        },
        {
          title: "LECTURA 8",
          text: "Protejamos a los niños del medio ambiente",
          to: "matematicas",
        },
        {
          title: "LECTURA 9",
          text: "LAS REDES SOCIALES",
          to: "matematicas",
        },
      ],
    };
  },
};
</script>
