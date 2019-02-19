<template>
    <div>
      <v-start-header/>
      <!-- <vheader v-bind="header"/> -->

        <v-container grid-list-md>
          <v-layout row wrap>
            
            <v-flex d-flex xs12 sm6 md6>
              <v-layout row wrap>
                <v-flex d-flex>
                  <v-card color="grey lighten-2">
                    <a href="modelljobb">
                      <v-img
                        class="white--text"
                        src="/images/IMG_5700.JPG"
                      >
                        <v-container fluid>
                          <v-layout>
                            <v-flex xs12 align-end flexbox>
                              <span class="headline">Modelljobb</span>
                            </v-flex>
                          </v-layout>
                        </v-container>
                      </v-img>
                    </a>
                  </v-card>
                </v-flex>

                <v-flex d-flex xs12>
                  <v-card color="grey lighten-2">
                    <v-card-title primary class="title">Rickard Broberg, lite mer än bara en Fitness Atlet</v-card-title>
                    <v-card-text>{{ bio }}</v-card-text>
                  </v-card>
                </v-flex>


                <v-flex d-flex>
                  <v-card color="grey lighten-2">
                    <a href="samarbeten">
                      <v-img
                        class="white--text"
                        src="/images/white-kit.jpg"
                      >
                        <v-container fluid>
                          <v-layout>
                            <v-flex xs12 align-end flexbox>
                              <span class="headline">Se alla samarbeten</span>
                            </v-flex>
                          </v-layout>
                        </v-container>
                      </v-img>
                    </a>
                  </v-card>
                </v-flex>

              </v-layout>
            </v-flex>


            <v-flex d-flex xs12 sm6 md6>
              <v-layout row wrap>
                
                <v-flex d-flex xs12>
                  <v-card color="grey lighten-2">
                    <a href="traningstips">
                      <v-img
                        class="white--text"
                        src="/images/IMG_5841.JPG"
                        height="500"
                      >
                        <v-container fluid>
                          <v-layout>
                            <v-flex xs12 align-end flexbox>
                              <span class="headline">Träningstips för nybörjare</span>
                            </v-flex>
                          </v-layout>
                        </v-container>
                      </v-img>
                    </a>
                  </v-card>
                </v-flex>

                <v-flex d-flex xs12>
                  <v-card color="grey darken-2">
                    <a href="tavlingar">
                      <v-img
                        class="white--text"
                        src="/images/IMG_4235.JPG"
                        height="700"
                      >
                        <v-container fluid>
                          <v-layout>
                            <v-flex xs12 align-end flexbox>
                              <span class="headline">Tävlingar</span>
                            </v-flex>
                          </v-layout>
                        </v-container>
                      </v-img>
                    </a>
                  </v-card>
                </v-flex>
                
                <v-flex d-flex>
                  <v-layout row wrap>
                    
                    <v-flex d-flex xs12>
                      <v-card color="grey lighten-2">
                        <v-card-text>{{ oneliner }}</v-card-text>
                      </v-card>
                    </v-flex>
                  </v-layout>
                </v-flex>


                <v-flex d-flex>
                  <v-card color="grey lighten-2">
                    <a href="kostrad/overnight-oat-with-proteinpowder">
                      <v-img
                        class="white--text"
                        src="/images/overnight-oat.jpg"
                        height="508"
                      >
                        <v-container fluid>
                          <v-layout>
                            <v-flex xs12 align-end flexbox>
                              <span class="headline">Overnight oat med elit nutrition</span>
                            </v-flex>
                          </v-layout>
                        </v-container>
                      </v-img>
                    </a>
                  </v-card>
                </v-flex>

              </v-layout>
            </v-flex>
            
            
          </v-layout>
        </v-container>

        <v-container grid-list-md text-xs-center>
          <v-layout row wrap>          
            <v-flex xl12>
              <v-card>
                <v-card-text class="pa-12">
                  <h2>Vill du komma i kontakt?</h2>
                  <p>Vill komma i kontakt så skicka endera ett direktmeddelande på Instagram <v-btn href="https://www.instagram.com/rickardbroberg" flat>@rickardbroberg</v-btn> eller skicka mig ett <v-btn href="mailto:rickard@rickardbroberg.se" flat>mail</v-btn></p>
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

      <vfooter/>
    </div>
</template>

<script>
import VStartHeader from '~/components/VStartHeader.vue'
import Vfooter from '~/components/VFooter.vue'

export default {
  data: function(){
    return {
      header: {
        title: 'Rickard Broberg',
        subheading: 'An fitness Athlete',
        image: 'header.jpg'
      },
      bio: `Jag är uppvuxen på landet utanför Örebro, men bor idag i Stockholm och jobbar som Senior Digital Marketing strategist, där jag hjälper kunderna med deras digitala kanaler i allt från strategi till teknisk utveckling. Där jag har en bakgrund som webbutvecklare`,
      oneliner: `RICKARDB15 ger dig 15% rabatt på ICANIWILL`
    }
  },
  components: {
    VStartHeader,
    Vfooter
  }
}
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: top;
  align-items: top;
  text-align: left;
}
.v-card a{
  text-decoration: none !important;
}

</style>

