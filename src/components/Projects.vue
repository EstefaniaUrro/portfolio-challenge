<template>
  <v-container>
    <v-card elevation="7" outlined class="rounded-lg  my-5 ">
      <v-card-title>Projects ({{ cards.length }})</v-card-title>
      <div class="px-2">
      <v-btn depressed outlined color="#4F4F4F"  class="ma-2"> HTML </v-btn>
       <v-btn depressed outlined color="#4F4F4F"  class="ma-2"> Vue </v-btn>
        <v-btn depressed outlined color="#4F4F4F"  class="ma-2"> React </v-btn>
      </div>
    </v-card>
    <v-card
      elevation="7"
      outlined
      class="d-flex align-content-center flex-wrap rounded-lg"
    >
      <v-container fluid>
        
        <v-row dense>
          <v-col v-for="card in cards" :key="card.title" :cols="4">
            <v-card>
              <v-img
                class="card-img black--text align-end"
                :src="card.src"
                height="300px"
              >
                <!--  -->
              </v-img>
              <v-card-title
                class="text-subtitle-1"
                v-text="card.tags"
              ></v-card-title>
             <v-card-title v-text="card.title"></v-card-title>
             <v-card-text class="text-body-2">
               {{card.description}}
             </v-card-text>
             <v-card-actions>
                <v-btn :href="card.demo" target="_blank" depressed color="primary" x-large md="6" class="ma-2" > DEMO </v-btn>
                <v-btn :href="card.git" target="_blank" depressed outlined color="primary" x-large md="6" class="ma-2" > CODE </v-btn>
             </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-card>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    cards: [
      {
        title: "Porfolio Challenge",
        code: 'Vue',        
        tags: "#Vue #Vuetify",
        src: "https://res.cloudinary.com/dae4jju6c/image/upload/v1644415389/portafolio/portafolio_bu5wop.png",
        description:"Descripcion del proyecto realizado con Vue y Vuetify ",
        demo:"",
        git:"",
      },
      {
        title: "GIF app",
        code: 'React',
        tags: "#React #CSS",
        src: "https://cdn.vuetifyjs.com/images/cards/road.jpg",
        description:"Descripcion del proyecto realizado con Vue y Vuetify ",
        demo:"https://estefaniaurro.github.io/gifapp/",
        git:"https://github.com/EstefaniaUrro/gifapp",
      },
      {
        title: "Heroes App",
        code: 'React',
        tags: "#React #Material UI",
        src: "https://cdn.vuetifyjs.com/images/cards/plane.jpg",
        description:"Descripcion del proyecto realizado con React y Material",
        demo:"https://hero-dc-marvel.herokuapp.com/",
        git:"https://github.com/EstefaniaUrro/hero-dc-marvel",
      },
    ],
  }),
};
</script>
