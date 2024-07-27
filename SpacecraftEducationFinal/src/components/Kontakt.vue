<template>
        <div class="background">
                <div class="background-image"></div>
                <div class="content ">

                        <h1>KONTAKT</h1>
                        SIE KÖNNEN UNS ZU ALLEN THEMEN KONTAKTIEREN!
                        <li>
                                FRAGEN ZU DEM PRODUKT
                        </li>
                        <li>
                                MIET- UND KAUFOPTIONEN
                        </li>

                        <li>PERSONLAISIERUNGEN</li>
                        ZÖGERNS SIE NICHT, UNS MIT IHREN FRAGEN ZU LÖCHERN.
                        KONTAKTINFORMATIONEN: info@spacecraft-education.com<br>
                        <button>READ MORE ABOUT US </button>
                </div>
        </div>
</template>

<script>
export default {
        name: 'Kontakt',

}
</script>

<style scoped>
.background-image {
        height: 100%;
        background-image: url("../assets/Kontakt_Photo2.png");
        background-size: 100% 100%;   /* TODO Anpassen an andere ScreenGrößen */
        background-repeat: no-repeat;
        filter: blur(8px);
}

.background {
        position: relative;
        min-height: var(--min-height-segment);
        height: 900px;
        /* width: 100%; */
}

.content {
        position: absolute;
        top: 5%;
        left: 10%;
}

button {
        position: relative;
        top: 50%;
        left: 50%;
        border: none;
        color: white;
        font-weight: var(--font-weight-bold);
        font-size: 20px;
        padding: 15px 32px;
        border-radius: 32px;
        background: #96B9D3;
}

button:hover {
        background: #7ab3e2;
        color: black;
        cursor: pointer;

}
</style>