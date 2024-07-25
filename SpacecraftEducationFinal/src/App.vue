<template>
  <div class="app-container NavGap">
    <NavBar />
    <IntroScreen />

    <InteraktivesLernen class="InteraktivesLernen" />
    <Angebot />
    <Kontakt />
    
    
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

<style scoped>


.app-container {
  overflow-x: hidden;
  width: 100%;
/*
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: var(--max-width-page);*/
  /* Set your desired max-width of page */
  /* Ensure the container takes full width up to max-width */
  /* Center the container */
}

.NavGap {
  margin-top: 170px;

}

.InteraktivesLernen {
  background-color: var(--background-color-secondary);
}
</style>
