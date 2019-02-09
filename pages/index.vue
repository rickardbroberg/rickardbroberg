<template>
    <div>
      <v-start-header/>
      <!-- <vheader v-bind="header"/> -->

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
                <v-flex d-flex>
                  <v-layout row wrap>
                    <v-flex d-flex xs12>
                      <v-card color="grey lighten-2" >
                        <v-img
                          class="white--text"
                          src="/images/IMG_5841.JPG"
                        >
                          <v-container fill-height fluid>
                            <v-layout fill-height>
                              <v-flex xs12 align-end flexbox>
                                <span class="headline">Träningstips för nybörjare</span>
                              </v-flex>
                            </v-layout>
                          </v-container>
                        </v-img>
                        <!-- <v-card-text>{{ lorem.slice(0, 40) }}</v-card-text> -->
                      </v-card>
                    </v-flex>
                    <v-flex d-flex xs12>
                      <v-card color="grey lighten-2">
                        <v-card-text>{{ lorem.slice(0, 40) }}</v-card-text>
                      </v-card>
                    </v-flex>
                  </v-layout>
                </v-flex>
              </v-layout>
            </v-flex>
            <v-flex d-flex xs12 sm6 md6 child-flex>
              <v-card color="grey darken-2">
                <v-img src="/images/IMG_5700.JPG"></v-img>
                <!-- <v-card-text>{{ lorem.slice(0, 90) }}</v-card-text> -->
              </v-card>
            </v-flex>
            <v-flex d-flex xs12 sm6 md6>
              <v-card color="grey lighten-2">
                <v-img
                  class="white--text"
                  src="/images/overnight-oat.jpg"
                >
                  <v-container fill-height fluid>
                    <v-layout fill-height>
                      <v-flex xs12 align-end flexbox>
                        <span class="headline">Overnight oat med elit nutrition</span>
                      </v-flex>
                    </v-layout>
                  </v-container>
                </v-img>
                <!-- <v-card-text>{{ lorem.slice(0, 100) }}</v-card-text> -->
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

        <v-container grid-list-md text-xs-center>
          <v-layout row wrap>          
            <v-flex xl12>
              <v-card>
                <v-card-text class="pa-12">
                  <h2>This is a heading</h2>
                  <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Vel neque at quos aperiam quaerat quidem atque illo illum, perspiciatis consequuntur tenetur ullam iure, similique voluptatibus, harum quisquam. Magni, iure veniam.</p>
                </v-card-text>
              </v-card>
            </v-flex>
          </v-layout>
        </v-container>

      <vfooter/>
    </div>
</template>

<script>
import Vue from 'vue'
import Vuetify from 'vuetify'

Vue.use(Vuetify, {
  iconfont: 'fa4'
})

import 'vuetify/dist/vuetify.min.css'
import 'font-awesome/css/font-awesome.min.css'

import Vheader from '~/components/VHeader.vue'
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
      lorem: `Lorem ipsum dolor sit amet, mel at clita quando. Te sit oratio vituperatoribus, nam ad ipsum posidonium mediocritatem, explicari dissentiunt cu mea. Repudiare disputationi vim in, mollis iriure nec cu, alienum argumentum ius ad. Pri eu justo aeque torquatos.`
    }
  },
  components: {
    Vheader,
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


</style>

