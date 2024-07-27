<template>
  <div class="app-container NavGap">
    <NavBar />
    <IntroScreen class="background-Intro" />

    <InteraktivesLernen class="InteraktivesLernen" />
    <Angebot class="Angebot" />
    
    <Kontakt class="Kontakt"/>


  </div>
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
  margin: 0;
  padding: 0;
  font-family: var(--font-style-normal);
}

.background-Intro {
  background-color: green;
}

.app-container {
  overflow-x: hidden;
  width: 100%;
}

.NavGap {
  margin-top: 170px;

}

.InteraktivesLernen {
  background-color: var(--background-color-secondary);
}


</style>
