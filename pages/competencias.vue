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
          title: "COMPETENCIA MATEMÁTICA",
          text: "0-35",
          to: "matematicas",
        },
        {
          title: "COMPETENCIA LECTORA",
          text: "0-60",
          to: "matematicas",
        },
        {
          title: "COMPETENCIA EN CIENCIAS EXPERIMENTALES",
          text: "0-60",
          to: "matematicas",
        },
      ],
    };
  },
};
</script>
