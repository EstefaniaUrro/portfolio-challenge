<template>
  <v-app class="app">
    <v-main>
      <v-container>
        <v-row no-gutters>
          <v-col md="12" sm="12">
            <About class="my-3" />
          </v-col>
          <v-col md="5" sm="12" xs="12" class="align-self-start" height="200">
            <Skills class="my-3"/>
            <v-row>
              <v-col md="12" xs="12">
              <Hobbies class="my-3"/>
              </v-col> 
            </v-row>
          </v-col>

          <v-col md="7" sm="12" xs="12" class="align-self-stretch">
            <Blog class="my-3"/>
            <Experiences class="my-3"/>
          </v-col>
          <v-col cols="12">
            <Projects class="my-3"/>
          </v-col>
          <Footer/>
        </v-row>
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
import "./assets/style.css";
import About from "./components/About";
import Skills from "./components/Skills";
import Hobbies from "./components/Hobbies";
import Blog from "./components/Blog";
import Experiences from './components/Experiences';
import Projects from './components/Projects';
import Footer from './components/Footer.vue';

export default {
  name: "App",

  components: {
    About,
    Skills,
    Hobbies,
    Blog,
    Experiences,
    Projects,
    Footer
  },

  data: () => ({
    //
  }),
};
</script>
