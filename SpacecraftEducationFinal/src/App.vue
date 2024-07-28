<template>
  <NavBar />
  <IntroScreen class="IntroScreen" />

  <InteraktivesLernen class="InteraktivesLernen" />
  <Angebot class="Angebot" />

  <Kontakt class="Kontakt" />


</template>

<script>
import NavBar from "./components/NavBar.vue";
import IntroScreen from "./components/IntroScreen.vue";
import InteraktivesLernen from "./components/InteraktivesLernen.vue";
import Angebot from "./components/Angebot.vue";
import Kontakt from "./components/Kontakt.vue";



export default {
  name: "App",
  components: {
    NavBar,
    IntroScreen,
    InteraktivesLernen,
    Angebot,
    Kontakt,

  },
};
</script>

<style>
body {
  margin: 0px;
  padding: 0px;
  font-family: var(--font-style-normal);
  overflow-x: hidden;
}

/* .background-Intro {
  background-color: green;
} */

.app-container {
  overflow-x: hidden;
  width: 100%;
  margin: 0;
  padding: 0;
}

.IntroScreen {
  margin: 0px;
}

.InteraktivesLernen {
  background-color: var(--background-color-secondary);
}
</style>
