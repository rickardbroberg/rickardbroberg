<template>
    <div>

      <vheader />

        <v-container grid-list-md mt-5>
          <v-layout row wrap>
            
            <v-flex d-flex xs12 sm6 md6>
              <v-card color="grey lighten-2">
                  <v-container fluid>
                    <v-layout>
                      <v-flex xs12 flexbox>
                        <span class="headline">Overnight oat med proteinpulver</span>
                        <p>Gör så här:</p>

                        <ul>
                          <li>Ta 1 del (jag kör 1 dl) proteinpulver, <br>förslagsvis <a target="_blank" href="http://www.elitstore.se/proteinpulver/elit-100-whey-isolate.html">Elit nutrition chokolate brownie</a></li>
                          <li>Ta 1 del havregryn (jag kör 1 eller 2 dl)</li>
                          <li>Blanda ihop med vatten till en något lös grötkonsistens</li>
                          <li>Strö på frysta bär, t.ex. hallon eller blåbär</li>
                          <li>Låt stå i kylskåpet över natten</li>
                        </ul>

                        <p>Ät kall på morgonen, enjoy!</p>

                      </v-flex>
                    </v-layout>
                  </v-container>
              </v-card>
            </v-flex>
            
            <v-flex d-flex xs12 sm6 md6>
                <v-img
                  class="white--text"
                  src="/images/overnight-oat.jpg"
                  height="500"
                >
                </v-img>
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
