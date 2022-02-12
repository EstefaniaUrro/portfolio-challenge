<template>
<v-container fluid >
        <v-row dense>
          <v-col v-for="card in cards" :key="card.title" md="4" sm="6" xs="12" class="my-sm-2" >
            <v-card>
              <v-img
                class="card-img black--text align-end"
                :src="card.src"
                :alt="card.title"
                height="300px"
              >
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
</template>

<script>
export default {
props: {
  cards: []
},
 data: () => ({
    
  }),
}
</script>
