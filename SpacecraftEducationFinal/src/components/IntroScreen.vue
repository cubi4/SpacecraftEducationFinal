<template>
        <div class="background">

                <h1>EIN STÜCK WELTRAUM IN DEINEN HÄNDEN</h1>
                <div class="flexbox flexbox-1">
                        <img src="../assets/Intro_Mädchen_Bau.png"
                                alt="Schülerin baut Satellit" />
                        <p class="text text-1">
                                Willkommen in der faszinierenden Welt
                                der
                                Raumfahrt mit
                                unserem Satellitenbaukasten! Unser
                                innovatives
                                Produkt ermöglicht es spielend zu
                                lernen, was
                                Satelliten
                                sind, wie sie aufgebaut sind, und welche
                                Aufgaben sie im
                                Weltraum übernehmen.
                        </p>
                        <img src="../assets/Intro_SatellitenBauKasten.png"
                                alt="Hilfe beim Satelliten bauen" />
                </div>
                <div class="flexbox flexbox-2">
                        <img src="../assets/Intro_Stefan_Bau.png"
                                alt="Zwei Satellit-Baukasten" />
                        <p class="text text-2">
                                Der Satellitenbaukasten besteht aus
                                3D-gedruckten
                                Satellitenmodellen in Originalgröße, die
                                aus
                                verschiedenen Satellitenkomponenten
                                bestehen und
                                selbstständig zusammengebaut werden
                                können.
                        </p>
                        <img src="../assets/Intro_Junge_Bau.png"
                                alt="Schüler baut Satelliten" />
                </div>
        </div>
</template>

<script>
export default {
        name: "IntroScreen",

}
</script>

<style scoped>
.background {
        background-image: url("../assets/Satellite_Background.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        padding: 0;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
}

h1 {
        font-size: var(--font-size-head);
        margin: 100px 0 70px 0;
}

.flexbox {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 4%;
        width: 100%;
}

.flexbox-1 {
        margin: 0px 0px 10px 0;
}

.flexbox-2 {
        padding: 100px 0px 20px 0;
}


.text {
        font-size: var(--font-size-normal);
        max-width: 400px;
        text-align: center;
        text-shadow: 1px 1px 2px black;
        /* maybe variable erstellen*/
}

img {
        min-width: 200px;
        width: 30%;
        /* maybe variable erstellen*/
        max-width: 600px;
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