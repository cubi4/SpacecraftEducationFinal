<template>
        <div class="background">
                <h1>INTERAKTIVES LERNEN</h1>
                <div class="flexbox flexbox-1">
                        <p class="text">
                                Der Satellitenbaukasten bietet eine einzigartige
                                Möglichkeit, die Form und Funktion von
                                Satelliten durch hands-on Erfahrung zu erlernen.
                                Jedes Modell enthält Bauteile, die vereinfacht
                                realen Satellitenkomponenten entsprechen.
                        </p>
                        <img src="../assets/Beispiel_Bild.png"
                                alt="BeispielLukas" />
                </div>
                <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
                <img src="../assets/Satellit_Explo_alpha.png"
                        alt="SatellitExplosion" />
                <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
        </div>
</template>

<script>
export default {
        name: 'InteraktivesLernen',
}
</script>

<style scoped>
.flexbox {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 4%;
        margin: 10px;
        width: 100%;

}


/* Macht text Sinn hier? */
.text {
        font-size: var(--font-size-normal);
        max-width: 700px;
        /* maybe variable erstellen*/
}

img {
        width: 30%;
        min-width: 200px;
        /* maybe variable erstellen*/
        max-width: 600px;
        /* irwie steuer ich gerade die größe vom Farbcontainer damit*/

        /* maybe variable erstellen*/
        border-radius: var(--border-radius-photo);
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