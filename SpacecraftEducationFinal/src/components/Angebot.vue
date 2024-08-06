<template>
        <div class="background">
                <h1>ANGEBOT</h1>
                <div class="flexbox">
                     
                              <div class="button flexbox-item-1"
                                    v-show="!isHovered1"
                                    @mouseover="hoverButton1"
                                    >
                                    <img class="icons"
                                                      src="../assets/Icon_shopping.png"></img><br>
                                          MIET- ODER KAUFOPTION
                                          DER<br>
                                          SATELLITENBAU-SETS
                              </div>
                        
                       
                              <div class="button button-2"
                                    v-show="isHovered1"
                                    @mouseleave="hoverButton1"
                                    >
                                    <div  class="littleHeader">
                                          <img id="littleShoppingBag" class="icons" src="../assets/Icon_shopping.png"> </img>
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
                 
                        <div 
                              class="button flexbox-item-3"
                               v-show="!isHovered2"
                                    @mouseover="hoverButton2" >

                                    <img class="icons" src="../assets/Icon_presentation.png"></img> <br>
                                    SCIENCETAINMENT-VORTRÄGE
                        </div>

                        <div class="button button-4"
                                    v-show="isHovered2"
                                    
                                    >
                                    <!-- <div  class="littleHeader">
                                          <img id="littleShoppingBag"  src="../assets/Icon_shopping.png"> </img>
                                          <p id="littleShoppingBagText"> MIET- ODER KAUFOPTION DER SATELLITENBAU-SETS </p>
                                    </div> -->
                                    <div class="flexbox-item-4">
                                          <Carousel id="carousel" :autoplay="2000"   >
                                                <Slide v-for="slide in 10" :key="slide">
                                                      <div class="carousel-item">
                                                            <img class="imagesInCarousel" id="image-1" src="../assets/Photocarousel/Rockets.jpg"> 
                                                            <img class="imagesInCarousel"  id="image-2" src="../assets/Photocarousel/RocketOutside1.jpg">
                                                      </div>
                                                </Slide>
                                                
                                                <template #addons>
                                                      <Pagination />
                                                </template>
                                          </Carousel>

                                          <p id="carouselText">Für eine vertiefte und unterhaltsame Erfahrung bieten wir die Möglichkeit Sciencetainment-Vorträge zu buchen. Unsere Expertinnen und Experten gewähren spannende Einblicke in die Welt der Raumfahrt und Satelliten, indem sie lebendige Vortragseinheiten, interaktive Experimente und Diskussionen durchführen. </p>
                                    </div>
                        </div>
                </div>
        </div>
</template>

<script>
import { Carousel, Navigation, Pagination, Slide } from 'vue3-carousel'
import 'vue3-carousel/dist/carousel.css'

export default {
        name: 'Angebot',
        components: {
            Carousel,
    Slide,
    Pagination,
    Navigation,
        },
        data() {
                return {
                        isHovered1: false,
                        isHovered2: false,
                        
                };
        },
        methods: {
                hoverButton1() {
                        this.isHovered1 = !this.isHovered1;
                        console.log("test");
                },
                hoverButton2() {
                        this.isHovered2 = !this.isHovered2;
                        console.log("test2");
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
.icons {
        width: 10%;
        margin: 2%
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

.button-4 {
      background-color: #96b9d3;
      width: 90%;
}

.flexbox {
        display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        gap: 50px;
        margin-top: 3%;
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
}

.flexbox-item-3 {
      display: flex;
        justify-content: center;
        flex-direction: column;
        align-items: center;
        background-color: #96b9d3;

        width: 70%;
        padding: 9.5% 0px;
        /* aspect-ratio: 1.78/1; */

}


.flexbox-item-4 {
      display: flex;
        justify-content: center;
        flex-direction: row;
        align-items: center;
        gap: 3%;
        /* margin: 0% 5% 5% 5% */
        border: 1px solid rgb(136, 255, 0);
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



/* ------------------------ Photocarousel ------------------------  */
#carousel{
      position: relative;
      border: 1px solid red;
      width: 50%;
}

.carousel-item {
  /* min-height: 200px; */
  width: 30%;
  background-color: var(--background-color-primary);
  color: white;
  font-size: 20px;
  border-radius: 8px;
  display: flex;
  justify-content: center;
  align-items: center;
}


.carousel__prev,
.carousel__next {
  box-sizing: content-box;
}

.imagesInCarousel {
      max-height: 500px;;
      max-width: 200px;

}

#image-2{

}

</style>