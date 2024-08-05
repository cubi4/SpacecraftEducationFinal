<template>
        <div class="background">
                <h1>ANGEBOT</h1>
                <div class="flexbox">
                     
                              <div class="button flexbox-item-1"
                                    v-show="!isHovered"
                                    @mouseover="hoverButton"
                                    >
                                    

                                          <img
                                                      src="../assets/Icon_shopping.png"></img><br>
                                          MIET- ODER KAUFOPTION
                                          DER<br>
                                          SATELLITENBAU-SETS
                                  
                              </div>
                        
                       
                              <div class="button button-2"
                                    v-show="isHovered"
                                    @mouseleave="leaveButton"
                                    >

                                    <div  class="littleHeader">
                                    <img id="littleShoppingBag"  src="../assets/Icon_shopping.png"> </img>
                                    <p id="littleShoppingBagText"> MIET- ODER KAUFOPTION DER SATELLITENBAU-SETS </p>
                              </div>
                                    <div class="flexbox-item-2">
                                          <video id="video"
                                                
                                                class="videoButton" autoplay loop muted>
                                                <source src="../assets/VideoButton.mp4"
                                                            type="video/mp4" />
                                          </video>

                                          <p id="videoText"> Wir bieten die Möglichkeit des Kaufs oder der Miete der Satellitenmodelle. Dies ermöglicht es, das Produkt sowohl langfristig zu besitzen als auch kurzfristig für Unterrichtseinheiten, Projekttage oder Veranstaltungen zu nutzen. </p>
                                    </div>
                              </div>
                 


                        <div class="button button-3">
                                <img
                                        src="../assets/Icon_presentation.png"></img><br>
                                SCIENCETAINMENT-VORTRÄGE
                        </div>
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
                        console.log("hover");

                },
                leaveButton() {
                        this.isHovered = false;
                        console.log("leave");
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
      margin: 30px 0px 0px 5%;
      

}

.button {
        border-radius: 20px;
        color: white;
        max-width: 2000px;

        /* aspect-ratio: 1.78/1; */
        /* anpassen sodass es VideoGröße entspricht */
        /* margin: 3%; */
        border: none;
        box-shadow: 0px 0px 20px #000000;
        font-size: var(--font-size-head);
}

.button-2{
      background-color: #100258;
      width: 90%;
      
}

.flexbox {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        gap: 50px;
}

.flexbox-item-1 {
      display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        background-color: #100258;
        width: 70%;
        padding: 9.5% 0px;
        /* aspect-ratio: 1.78/1; */

}

.flexbox-item-2 {
      display: flex;
        justify-content: center;
        flex-direction: row;
        align-items: center;
        gap: 3%;
      
        margin: 0% 5% 5% 5%

      /* padding: 5%; */

      
}

.littleHeader {

      display: flex;
      justify-content: flex-start;
        flex-direction: row;
        align-items: center;

}

#littleShoppingBag {
      width: 4%;
}

#littleShoppingBagText {
      font-size: var(--font-size-normal);

}

#videoText {
      font-size: var(--font-size-normal);

}

#video{
      width: 60%;
      object-fit: contain;
}


.button-3 {
        background-color: #96b9d3;
}


video {
        width: 70%;
        border-radius: 20px;
}

img {
        width: 10%;
        margin: 2%
}
</style>