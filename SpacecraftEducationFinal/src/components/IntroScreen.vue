<template>
        <h1>"Ein Stück Weltraum in deinen Händen"</h1>
        <div class="flexbox flexbox-1">
                <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
                <p class="text text-1">
                        Willkommen in der faszinierenden Welt der Raumfahrt mit
                        unserem Satellitenbaukasten! Unser innovatives
                        Produkt ermöglicht es spielend zu lernen, was Satelliten
                        sind, wie sie aufgebaut sind, und welche Aufgaben sie im
                        Weltraum übernehmen.
                </p>
                <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
        </div>
        <div class="flexbox flexbox-1">
                <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
                <p class="text text-2">
                        Der Satellitenbaukasten besteht aus 3D-gedruckten
                        Satellitenmodellen in Originalgröße, die aus
                        verschiedenen Satellitenkomponenten bestehen und
                        selbstständig zusammengebaut werden können.
                </p>
                <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
        </div>
</template>

<script>
export default {
        name: "IntroScreen",

}
</script>

<style scoped>
.flexbox {
        display: flex;
        align-items: center;
        gap: 4%;
        margin: 10px;
}

.text {
        font-size: var(--font-size-normal);
        max-width: 500px; /* maybe variable erstellen*/
}

img {
        width: 30%; 
        min-width: 200px; /* maybe variable erstellen*/
        max-width: 400px; /* maybe variable erstellen*/
        border-radius: 20px;
}

/* ---------------------------Animation--------------------------- */

@keyframes fadeInLeft {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}

h1 {
  animation: fadeInLeft 2s ease-in-out forwards;
}
</style>