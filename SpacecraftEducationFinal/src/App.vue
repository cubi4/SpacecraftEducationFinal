<template>
  <div class="app-container NavGap">
    <NavBar />
    <IntroScreen />

    <InteraktivesLernen class="InteraktivesLernen" />
    <Angebot />

  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import IntroScreen from "./components/IntroScreen.vue";
import InteraktivesLernen from "./components/InteraktivesLernen.vue";
import Angebot from "./components/Angebot.vue";

export default {
  name: "App",
  components: {
    NavBar,
    IntroScreen,
    InteraktivesLernen,
    Angebot
  },
};
</script>

<style scoped>
.app-container {
  border: 1px solid red;

  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: var(--max-width-page);
  /* Set your desired max-width of page */
  width: 100%;
  /* Ensure the container takes full width up to max-width */
  margin: 0 auto;
  /* Center the container */
}

.NavGap {
  margin-top: 170px;
}

.InteraktivesLernen {
  background-color: var(--background-color-secondary);
}
</style>
