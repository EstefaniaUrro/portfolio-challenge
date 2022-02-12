<template>
  <v-container>
    <v-card class="pa-4 rounded-lg" elevation="7" outlined>
      <v-card-text class="text-sm-h5"> Skills </v-card-text>
    <v-card class="rounded-lg d-flex  pa-4" elevation="0" >
      <v-row>
        <v-col md="12" sm="12" xs="12">
          <div class="d-inlineblock d-flex flex-row">
            <span>HTML/5</span> 
            <v-progress-linear
          value="95"
          height="12"
          rounded
          class="skill-bar ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
          </div>
          <div class="d-inlineblock d-flex flex-row">
            <span>CSS/3</span> 
            <v-progress-linear
          value="95"
          height="12"
          rounded
          class="skill-bar ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
          </div>
          <div class="d-inlineblock d-flex flex-row">
             <span>JAVASCRIPT</span>
            <v-progress-linear
          value="75"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
          </div>
           <div class="d-inlineblock d-flex flex-row">
          <span>JAVA</span>
          <v-progress-linear
          value="80"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
        </div>
        <div class="d-inlineblock d-flex flex-row">
          <span>REACT</span>
           <v-progress-linear
          value="65"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
        </div>
        <div class="d-inlineblock d-flex flex-row">
          <span>VUE</span>
           <v-progress-linear
          value="65"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear> 
        </div>
        </v-col>
        <!-- <v-col md="6" sm="12" xs="12">
        <div class="d-inlineblock d-flex flex-row">
          <span>JAVA</span>
          <v-progress-linear
          value="80"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
        </div>
        <div class="d-inlineblock d-flex flex-row">
          <span>REACT</span>
           <v-progress-linear
          value="65"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
        </div>
        <div class="d-inlineblock d-flex flex-row">
          <span>VUE</span>
           <v-progress-linear
          value="65"
          height="12"
          rounded
          class="skill-bar mt-2 ma-2"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear> 
        </div>
        </v-col> -->
      </v-row>
     </v-card>

    </v-card>
  </v-container>
</template>

<script>
export default {
  name: "Skills",
  data: () => ({
  }),
};
</script>
