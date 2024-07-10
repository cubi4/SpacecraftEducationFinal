<template>
  <div class='app-container'>
  <div class="NavGap">
    <NavBar />
  </div>
  
  <IntroScreen />
</div>
  


</template>



<script>
import NavBar from './components/NavBar.vue';
import IntroScreen from './components/IntroScreen.vue';

export default {
  name: 'App',
  components: {
    NavBar,
    IntroScreen
  }
}

</script>

<style scoped>
.app-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: var(--max-width-page); /* Set your desired max-width of page */
  width: 100%; /* Ensure the container takes full width up to max-width */
  margin: 0 auto; /* Center the container */
}


.NavGap {
  margin-top: 170px;
}

</style>
