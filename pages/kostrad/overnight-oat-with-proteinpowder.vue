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
                        <span class="headline">Äts kall med ett glas lättmjölk</span>
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
                          <v-flex xs12 flexbox>
                            <span class="headline">Recept: overnight oat med proteinpulver</span>
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
        title: 'Recept: overnight oat med proteinpulver',
        subheading: 'Borde det vara ens en header haer',
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
