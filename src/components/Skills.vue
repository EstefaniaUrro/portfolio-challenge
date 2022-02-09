<template>
  <v-container>
    <!-- <v-row no-gutters>
      <v-col cols="4"> -->
    <v-card class="pa-4 rounded-lg d-flex" elevation="7" outlined>
      <v-card max-width="150" elevation="0">
        <div class="d-inlineblock">HTML/5</div>
        <div class="d-inlineblock">CSS/3</div>
        <div class="d-inlineblock">JAVASCRIPT</div>
        <div class="d-inlineblock">JAVA</div>
        <div class="d-inlineblock">REACT</div>
        <div class="d-inlineblock">VUE</div>
      </v-card>
      <v-card class="bar mx-2" elevation="0">
        <v-progress-linear
          value="95"
          height="12"
          rounded
          class="skill-bar mt-2 mb-3"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>

        <v-progress-linear
          value="95"
          height="12"
          rounded
          class="skill-bar mt-2 mb-3"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>

        <v-progress-linear
          value="75"
          height="12"
          rounded
          class="skill-bar mt-2 mb-3"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>

        <v-progress-linear
          value="80"
          height="12"
          rounded
          class="skill-bar mt-2 mb-3"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>

        <v-progress-linear
          value="65"
          height="12"
          rounded
          class="skill-bar mt-2 mb-3"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>

        <v-progress-linear
          value="65"
          height="12"
          rounded
          class="skill-bar mt-2 mb-3"
          color="primary"
          background-color="grey lighten-1"
        ></v-progress-linear>
      </v-card>
    </v-card>
    <!-- </v-col>
    </v-row> -->
  </v-container>
</template>

<script>
export default {
  name: "Skills",
  data: () => ({
    power: 65,
  }),
};
</script>
