<template>
        <div class="background">
                <h1>KONTAKT</h1>
                <p class="text">
                        SIE KÖNNEN UNS ZU ALLEN THEMEN KONTAKTIEREN!</p>
                <li>
                        <ul class="text">FRAGEN ZU DEM PRODUKT</ul>
                </li>
                <li>
                        <ul class="text">MIET- UND KAUFOPTIONEN</ul>
                </li>

                <li>
                        <ul class="text">PERSONLAISIERUNGEN</ul>
                </li>
                <p class="text"> ZÖGERN SIE NICHT, UNS MIT IHREN FRAGEN ZU
                        LÖCHERN.
                        KONTAKTINFORMATIONEN: info@spacecraft-education.com</p>

                <div class="content">
                        <button>READ MORE ABOUT US </button>
                        <div class="banner">
                                <span class="item1">HIER LAUFEN DANN
                                        EMPFEHLUNGEN UND
                                        SO
                                        DURCH</span>
                                <span class="item2">UND HIER IST EIN ANDERER
                                        TEXT</span>
                        </div>
                </div>
        </div>
</template>

<script>
export default {
        name: 'Kontakt',

}
</script>

<style scoped>
.background {
        background-image: url("../assets/Kontakt_Photo.png");
        background-size: cover;
        background-repeat: no-repeat;
        min-height: 100vh;
        display: flex;
        flex-direction: column;
        margin-bottom: 0px;
}

h1 {
        font-size: var(--font-size-head);
        padding-top: 30px;
}

.text {
        font-size: var(--font-size-normal);
        text-shadow: 1px 1px 2px black;
}

.content {
        margin-top: 400px;
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 30px;
        margin-bottom: 50px;
}

button {
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

.banner {
        background-color: var(--background-color-primary);
        font-size: var(--font-size-normal);
        width: 40%;
        min-height: 80px;
        border-radius: 20px;
        margin-top: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
}


/* -------------------------------Animation------------------------------- */

.banner {
        white-space: nowrap;
        position: relative;
        overflow: hidden;
}

span {
        animation: runText 6s linear infinite;
        position: absolute;
        left: 100%;
}

.item1 {
        animation-delay: 0s;
}

.item2 {
        animation-delay: 3.5s;
}



@keyframes runText {
        to {
                left: -100%;
        }
}
</style>