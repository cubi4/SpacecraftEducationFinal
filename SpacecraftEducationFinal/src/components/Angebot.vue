<template>
        <div class="background">
                <h1>ANGEBOT</h1>
                <div class="flexbox">
                        <button class="button button-1">
                                <img src="../assets/Icon_shopping.png"></img><br>
                                MIET- ODER KAUFOPTION
                                DER<br>
                                SATELLITENBAU-SETS</button>

                        <button class="button button-2">
                                <img src="../assets/Icon_presentation.png"></img><br>
                                SCIENCETAINMENT-VORTRÄGE
                        </button>
                </div>
        </div>
</template>

<script>
export default {
        name: 'Angebot',

}
</script>

<style scoped>

.background {
        min-height: var(--min-height-segment);
        background-color: var(--background-color-primary);
}

.flexbox {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        gap: 50px;
}

button {
        background-color: aqua;
        border-radius: 20px;
        max-width: 2000px;
        width: 70%;
        aspect-ratio: 2/1;
        margin: 3%;
        border: none;
        box-shadow: 0px 0px 20px #000000;
        font-size: var(--font-size-head);
}

.button-1 {
        background-color: #100258;
        margin-bottom: 1%;
}
.button-2 {
        background-color: #96b9d3;
}

img {
        width: 10%;
        margin: 2%
}
</style>