<template>
  <v-container>
    <v-card elevation="7" outlined class="rounded-lg my-5">
      <v-card-text class="text-sm-h5"> Projects ({{ cards.length }}) </v-card-text>
      <div class="px-2">
        <v-btn
          depressed
          outlined
          v-on:click="handleHTML"
          class="ma-2 black--text"
          v-bind:class="{html: isActiveH}"
        >
          HTML
        </v-btn>
        <v-btn
          depressed
          outlined
          v-on:click="handleVue"
          class="ma-2 black--text"
             v-bind:class="{vue: isActiveV}"
        >
          Vue
        </v-btn>
        <v-btn 
          
          outlined
          v-on:click="handleReact"
          class="ma-2 black--text"
          v-bind:class="{react: isActiveR}"
        >
          React
        </v-btn>
      </div>
    </v-card>
    <v-card
      elevation="7"
      outlined
      class="d-flex align-content-center flex-wrap rounded-lg"
      v-if="project"
    >
      <projects-search :cards="arrCard" />
    </v-card>
  </v-container>
</template>

<script>
import ProjectsSearch from "./ProjectsSearch.vue";
// import axios from "axios";
import data from "../assets/data.json";
export default {
  components: { ProjectsSearch },
  data() {
    return {
      project: false,
      arrCard: [],
      cards: data.cards,
      isActiveH: false,
      isActiveV: false,
      isActiveR: false
    };
  },
  methods: {
    created() {
      this.project = false;
    },
    handleHTML: function () {
      this.isActiveV = false;
      this.isActiveR = false;
      if (!this.cards.length) {
        console.log("No hay anda");
        this.project = false;
      } else {
        this.arrCard = this.cards.filter((cards) => {
          return cards.code == "HTML";
        });
        if (this.arrCard.length) {
          this.project = true;
         this.isActiveH = true;
        } else {
          this.project = false;
            console.log("No hay anda");
        }
      }
    },
    handleVue: function () {
      this.isActiveH = false;
      this.isActiveR = false;
      if (!this.cards.length) {
        this.project = false;
      } else {
        this.arrCard = this.cards.filter((cards) => {
          return cards.code == "Vue";
        });
        if (this.arrCard.length) {
          this.project = true;
          this.isActiveV = true;
        } else {
          this.project = false;
        }
      }
    },
    handleReact: function () {
     this.isActiveV = false;
      this.isActiveH = false;
     if (!this.cards.length) {
        console.log("No hay anda");
        this.project = false;
      } else {
        this.arrCard = this.cards.filter((cards) => {
          return cards.code == "React";
        });
        if (this.arrCard.length) {
          this.project = true;
           this.isActiveR = true;
        } else {
          this.project = false;
        }
      }
      
    },
  },
};
</script>
