<template>
  <v-container>
    <v-card
      elevation="7"
      outlined
      class="d-flex align-content-center flex-wrap rounded-lg"
    >
      <v-row no-gutters>
        <v-col md="3" sm="5" xs="7" class="ma-3 text-center">
          <v-avatar class="rounded-lg ma-auto align-sm-center" size="150" tile>
            <v-img src="https://res.cloudinary.com/dae4jju6c/image/upload/v1644415389/portafolio/logo_estefania_wacody.png"></v-img>
          </v-avatar>
        </v-col>
        <v-col md="5" sm="6" xs="12" class="my-3 pa-1 mx-sm-3">
          <div class="text-h4 text--primary my-1">Estefania Urro Vasquez</div>
          <div class="subtitle-2 mb-2">Junior web developer</div>
          <div class="body-2 mr-2">
            Self-motivated developer, who is willing to learn and
            createoutstanding <br />
            UI applications.<br />
            Donec aliquam est dui, vel vestibulum diam sollicitudin id. Quisque
            <br />feugiat malesuada molestie.
          </div>
        </v-col>
        <v-col md="3" sm="5" xs="12" class="my-3">
          <div>
            <p class="px-3">
              <v-icon medium> mdi-email </v-icon> urroestefania@gmail.com
            </p>
            <p class="px-3">
              <v-icon medium> mdi-phone </v-icon> (+34) 623 37 2593
            </p>
          </div>
        </v-col>
      </v-row>
    </v-card>
   
  </v-container>
</template>

<script>
export default {
  name: "About",

  data: () => ({}),
};
</script>
