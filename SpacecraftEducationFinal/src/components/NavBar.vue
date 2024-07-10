<template>

        <div class="wrapper">
                <div class="icon item-1">
                        <img src="\Logo_Inverted.svg">
                </div>
                <div class="text button item-2">
                        Was machen wir?
                </div>
                <div class="text button item-3">
                        Unsere Produkte
                </div>
                <div class="text button item-4">
                        Unser Kontakt
                </div>
                <div class="text item-5 rightsideText">
                        Ein Stück Weltraum in deinen Händen
                </div>
        </div>

</template>

<script>
export default {
        name: "NavBar",
}
</script>

<style scoped>
.wrapper {
        /* Center and fix NavBar at top */
        position: fixed;
        top: 0;
        left: 0;
        /* for center Navbar after certain width*/
        /* for center Navbar after certain width*/
        right: 0;
        z-index: 1000;
        /* Give Navbar right Properties */
        display: flex;
        align-items: center;
        justify-content: start;
        gap: 6%;
        background-color: rgba(35, 37, 72, 0.8);
        height: 70px;
        border-radius: 30px;
        margin: 30px 20px 0 20px;
        box-shadow: 0px 4px 4px 0px rgba(0, 0, 0, 0.25);
        backdrop-filter: blur(5px);
}

.text {
        position: relative;
        color: white;
        font-size: var(--font-size-normal);
        margin: 0 5px;
}

.rightsideText {
        font-size: 20px;
}

.rightsideText {
        width: 200px;
        margin-left: auto;
        margin-right: 20px;
        text-align: center;
}

img {
        width: 150px;
        margin: 0 25px;
}

/* -----------------------------Hover effects----------------------------- */

.button {
        position: relative;
}

.button:hover {
        color: #96b9d3;
        cursor: pointer;
}

.button::after {
        content: '';
        position: absolute;
        left: 0;
        bottom: -8px;
        /*distance underline to text*/
        height: 3px;
        /* thickness underline */
        border-radius: 2px;
        background-color: #96b9d3;
        transition: width 0.3s ease;
}

.button:hover::after {
        width: 60%;
        /* length of line */
        left: 20%;
        /* left= 100-width/2 */
}
</style>
