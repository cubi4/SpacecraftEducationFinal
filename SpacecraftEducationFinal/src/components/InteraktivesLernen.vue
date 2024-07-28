<template>
        <div class="background">
                <h1>INTERAKTIVES LERNEN</h1>
                <div class="wrapper">
                        <div class="outer-flexbox">
                                <div class="column inner-flexbox-left">
                                        <p class="text item item-1">
                                                Der Satellitenbaukasten bietet
                                                eine
                                                einzigartige
                                                Möglichkeit, die Form und
                                                Funktion von
                                                Satelliten durch hands-on
                                                Erfahrung zu
                                                erlernen.
                                                Jedes Modell enthält Bauteile,
                                                die
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
        </div>
</template>

<script>
export default {
        name: 'InteraktivesLernen',
}
</script>

<style scoped>
h1 {
        flex: 1 1 100%;
        font-size: var(--font-size-head);
        margin: 0px;
}

.background {
        padding-top: 30px;
        min-height: var(--min-height-segment);
        display: flex;
        justify-content: center;
        flex-wrap: wrap;
}

.wrapper{
        border: 1px solid black;
        max-width: var(--max-width-page);
        width: 100%;
}
.outer-flexbox {
        display: flex;
        justify-content: center;
        width: 100%;
        gap: 3%;
        padding-bottom: max(3%, 50px);
        padding-left: 3%;

}

.inner-flexbox-left {
        border: 1px solid black;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        /* width: 100%; */
}

.inner-flexbox-right {
        border: 1px solid black;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        /* width: 100%; */
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
        width: 60%;
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