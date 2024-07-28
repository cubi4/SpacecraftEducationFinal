<template>
        <div class="background">
                <h1>ANGEBOT</h1>
                <div class="flexbox">
                        <button @mouseover="hoverButton"
                                @mouseleave="leaveButton"
                                class="button button-1">
                                <div v-show="!isHovered">

                                        <img
                                                src="../assets/Icon_shopping.png"></img><br>
                                        MIET- ODER KAUFOPTION
                                        DER<br>
                                        SATELLITENBAU-SETS
                                </div>
                                <video v-show="isHovered"
                                        @mouseleave="leaveButton"
                                        @click="clickedButton"
                                        class="videoButton" autoplay loop muted>
                                        <source src="../assets/VideoButton.mp4"
                                                type="video/mp4" />
                                </video>
                        </button>

                        <button class="button button-2">
                                <img
                                        src="../assets/Icon_presentation.png"></img><br>
                                SCIENCETAINMENT-VORTRÄGE
                        </button>
                </div>
        </div>
</template>

<script>

export default {
        name: 'Angebot',
        components: {
        },
        data() {
                return {
                        isHovered: false,
                };
        },
        methods: {
                hoverButton() {
                        this.isHovered = true;
                },
                leaveButton() {
                        this.isHovered = false;
                },
                clickedButton() {
                        console.log('clicked');
                },
        },
};
</script>

<style scoped>
.background {
        min-height: var(--min-height-segment);
        background-color: var(--background-color-primary);
}

h1{
        font-size: var(--font-size-head);
}


.flexbox {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        gap: 50px;
}


button {
        border-radius: 20px;
        color: white;
        max-width: 2000px;
        width: 70%;
        aspect-ratio: 1.78/1;
        /* anpassen sodass es VideoGröße entspricht */
        margin: 3%;
        border: none;
        box-shadow: 0px 0px 20px #000000;
        font-size: var(--font-size-head);
}

.button-1 {
        position: relative;
        background-color: #100258;
        margin-bottom: 1%;
}

.button-2 {
        background-color: #96b9d3;
}


video {
        width: 100%;
        border-radius: 20px;
}

img {
        width: 10%;
        margin: 2%
}
</style>