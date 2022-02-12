<template>
  <v-container>
    <v-card
      elevation="7"
      outlined
      class="d-flex flex-wrap align-content-center rounded-lg pa-md-5 pa-sm-10">
      <v-row no-gutters>
        <v-col  md="2" sm="5" xs="1"  class="ma-md-auto mx-sm-auto about-img">
          <!-- <v-avatar class="rounded-lg about-img red" > -->
            <v-img class="about-img-img"  src="https://res.cloudinary.com/dae4jju6c/image/upload/v1644415389/portafolio/logo_estefania_wacody.png"></v-img>
          <!-- </v-avatar> -->
        </v-col>
        <v-col  md="8" sm="11" xs="4" class="my-3 pa-md-1 mx-sm-5">
         <v-list
          subheader
          max-width="100%">
         <v-list-item>
          <v-list-item-content>
            <v-list-item-title>Estefania Urro Vasquez</v-list-item-title>
            <v-list-item-subtitle>Junior web developer</v-list-item-subtitle>
            <!-- <v-list-item-action-text> Self-motivated developer, who is willing to learn and createoutstanding UI applications.<br />
            Donec aliquam est dui, vel vestibulum diam sollicitudin id. Quisque
            <br />feugiat malesuada molestie.</v-list-item-action-text> -->
          </v-list-item-content>
          <v-list-item-action>
              <v-list-item-title><v-icon medium> mdi-email </v-icon> urroestefania@gmail.com</v-list-item-title>
              <v-list-item-title><v-icon medium> mdi-phone </v-icon> (+34) 623 37 2593</v-list-item-title>
          </v-list-item-action>
        </v-list-item>

        <v-list-item>
          <v-list-item-content>
            <v-list-item-text> Self-motivated developer, who is willing to learn and createoutstanding UI applications.
            <br />
            Donec aliquam est dui, vel vestibulum diam sollicitudin id. Quisque feugiat malesuada molestie.</v-list-item-text>
          </v-list-item-content>         
        </v-list-item>
         </v-list>
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
