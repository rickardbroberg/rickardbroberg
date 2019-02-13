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
                <v-card-title primary class="title">Lorem</v-card-title>
                <v-card-text>{{ lorem }}</v-card-text>
              </v-card>
            </v-flex>
            <v-flex d-flex xs12 sm6 md6>
              <v-layout row wrap>
                <v-flex d-flex>
                  <v-card color="grey lighten-2">
                    <v-img
                      class="white--text"
                      src="/images/white-kit.jpg"
                    >
                      <v-container fill-height fluid>
                        <v-layout fill-height>
                          <v-flex xs12 align-end flexbox>
                            <span class="headline">Se alla samarbeten</span>
                          </v-flex>
                        </v-layout>
                      </v-container>
                    </v-img>
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
