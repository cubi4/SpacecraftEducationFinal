<template>
        <div class="background">
                <h1>INTERAKTIVES LERNEN</h1>
                <div class="outer-flexbox">
                        <div class="column inner-flexbox-left">
                                <p class="text item item-1">
                                        Der Satellitenbaukasten bietet eine
                                        einzigartige
                                        Möglichkeit, die Form und Funktion von
                                        Satelliten durch hands-on Erfahrung zu
                                        erlernen.
                                        Jedes Modell enthält Bauteile, die
                                        vereinfacht
                                        realen Satellitenkomponenten
                                        entsprechen.
                                </p>

                                <img class="item item-2"
                                        src="../assets/Interaktives_Lernen_Personen_Bau.png"
                                        alt="BeispielLukas" />
                        </div>


                        <div class="column inner-flexbox-right">
                                <img class="item item-3"
                                        src="../assets/Satellit_Explo_alpha.png"
                                        alt="SatellitExplosion" />
                        </div>

                </div>
        </div>
</template>

<script>
export default {
        name: 'InteraktivesLernen',
}
</script>

<style scoped>
h1 {
        font-size: var(--font-size-head);
        margin: 0px;
}

.background {
        padding-top: 30px;
      min-height: var(--min-height-segment);
}

.outer-flexbox {
        display: flex;
        justify-content: center;
        width: 100%;
        gap: 12%;
        margin: 10px;

}

.inner-flexbox-left {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
}

.inner-flexbox-right {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
}


/* .item{
        flex-basis: 50%;
        box-sizing: border-box;
} */
/* Macht text Sinn hier? */
.text {
        font-size: var(--font-size-normal);
        max-width: 700px;
        /* maybe variable erstellen*/
}

img {
        width: 80%;
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