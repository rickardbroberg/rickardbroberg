<template>
    <div>
      <vheader v-bind="header"/>

        <v-container grid-list-md>
          <v-layout row wrap>
            <v-flex d-flex xs12 sm6 md6>
              <v-card color="grey lighten-2">
                <v-img
                  class="white--text"
                  src="/images/IMG_4235.JPG"
                >
                  <v-container fill-height fluid>
                    <v-layout fill-height>
                      <v-flex xs12 align-end flexbox>
                        <span class="headline">Tävlingar</span>
                      </v-flex>
                    </v-layout>
                  </v-container>
                </v-img>
              </v-card>
            </v-flex>
            <v-flex d-flex xs12 sm6 md6>
              <v-layout row wrap>
                <v-flex d-flex>
                  <v-card color="grey lighten-2">
                      <v-container fill-height fluid>
                        <v-layout fill-height>
                          <v-flex xs12 align-end flexbox>
                            <span class="headline">Lär dig chins eller pullups</span>
                            <p>Först kan vi ta en rad om chins eller pullups, i Sverige verkar man säga chins, och i USA pullups. Jag personligen säger chins, pullups är för mig en annan grej och det kan ni <a href="">läsa här</a></p>
                            
                            <p>Skillnaden mellan chins och pullups är för mig greppningen av baren med händerna.</p>

                            <p> !! BILD SOM VISAR SKILLNADEN !!</p>

                            <p>Har du en längtan efter att kunna göra chins, men vet inte hur du ska träna för att komma dit? Jag ska nu försöka ge mina bästa tips, som jag hoppas kan inspirera och hjälpa dig på vägen! Mitt första tips är att träna på negativa chins.</p>
                            
                            <h2>Vad är negativa chins?</h2>
                            <p>Med negativa chins innebär det att man gör chins rörelsen baklänges, man börjar d.v.s. högst upp och sänker sig sakta neråt, här gäller det att hålla emot så mycket man kan för bästa effekt.</p>

                            <h2>Chins med gummiband</h2>

                            <p>Ett annat bra tips är också att göra chins med gummiband, där man då fäster gummibandet runt baren, och sedan placerar in ena foten. På så sätt får man en elastisk draghjälp i början som sedan avtar ju högre upp emot baren man kommer.</p>
                          </v-flex>
                        </v-layout>
                      </v-container>
                    
                    <!-- <v-card-text>{{ lorem.slice(0, 70) }}</v-card-text> -->
                  </v-card>
                </v-flex>
                
              </v-layout>
            </v-flex>
            
            
          </v-layout>
        </v-container>
      
      <vfooter/>
    </div>
</template>

<script>
import Vheader from '~/components/VHeader.vue'
import Vfooter from '~/components/VFooter.vue'

export default {
  data: function(){
    return {
      header: {
        title: 'Chins eller pullups',
        subheading: 'Hitta inspiration och tips till övrningar',
        image: 'traningstips.jpg'
      },
      lorem: 'lorem text'
    }
  },
  components: {
    Vheader,
    Vfooter
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;  
}

</style>
