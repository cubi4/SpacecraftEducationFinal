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
        data() {
        }
}
</script>

<style scoped>
.wrapper {
        /* position: relative; */
        display: flex;
        align-items: center;
        justify-content: start;
        gap: 6%;
        background-color: #232548;
        height: 90px;
        border-radius: 33px;
        margin: 30px 20px 0 20px;
}

.text {
        position: relative;
        color: white;
        font-size: 20px;
        margin: 0 5px;
}

.rightsideText {
        width: 200px;
        margin-left: auto;
        margin-right: 20px;
        text-align: center;
}

img {
        width: 190px;
        margin: 0 20px;
}



.button{
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
        bottom: -6px; /*distance underlin to text*/
        height: 2px; /* thickness underline */
        background-color: #96b9d3;
        transition: width 0.3s ease;
}

.button:hover::after {
  width: 70%; /* length of line */
  left: 15%; /* left= 100-width/2 */
}

</style>