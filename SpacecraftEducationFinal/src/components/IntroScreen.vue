<template>
        <div class="background">

                <h1>"Ein Stück Weltraum in deinen Händen"</h1>
                <div class="flexbox flexbox-1">
                        <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
                        <p class="text text-1">
                                Willkommen in der faszinierenden Welt der
                                Raumfahrt mit
                                unserem Satellitenbaukasten! Unser innovatives
                                Produkt ermöglicht es spielend zu lernen, was
                                Satelliten
                                sind, wie sie aufgebaut sind, und welche
                                Aufgaben sie im
                                Weltraum übernehmen.
                        </p>
                        <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
                </div>
                <div class="flexbox flexbox-1">
                        <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
                        <p class="text text-2">
                                Der Satellitenbaukasten besteht aus
                                3D-gedruckten
                                Satellitenmodellen in Originalgröße, die aus
                                verschiedenen Satellitenkomponenten bestehen und
                                selbstständig zusammengebaut werden können.
                        </p>
                        <img src="../assets/Beispiel_Bild.png" alt="BeispielLukas" />
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
        background-image: url("../assets/Satellite_Background.png");
        /* background-color: green; */
}

.flexbox {
        display: flex;
        justify-content: center;
        align-items: center;
        gap: 4%;
        margin: 10px;
        width: 100%;
}

.text {
        font-size: var(--font-size-normal);
        max-width: 400px;
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