<template>
    <div>
      <v-start-header/>
      <!-- <vheader v-bind="header"/> -->
      <sidebar/>
    

        <v-container grid-list-md>
          <v-layout align-end wrap frontbox>
            <v-flex v-for="item in frontboxes" :key="`4${item}`" xs4>
              <v-card dark :color="item.color">
                <v-card-title primary-title>
                  <div>
                    <h3 class="headline mb-0">{{item.title}}</h3>
                    <div>{{item.premble}}</div>
                  </div>
                </v-card-title>
                <v-card-actions>
                  <v-btn :href="item.url" block :color="item.btnColor">{{item.button}}</v-btn>
                </v-card-actions>
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
      frontboxes: [
        {
          title: 'OVER NIGHT OATS',
          premble: 'Letar du efter en fitnessfrukost? Denna är baserad på proteinpulver och havregryn...',
          button: 'Läs receptet',
          url: 'kostrad',
          color: 'light-blue darken-1',
          btnColor: 'light-blue darken-4'
        },
        {
          title: 'LÄR DIG GÖRA CHINS',
          premble: 'Här får du mina bästa tips för att lära dig göra chins eller pullups...',
          button: 'Läs mina tips',
          url: 'traningstips',
          color: 'teal darken-1',
          btnColor: 'teal darken-4'
        },
        {
          title: 'ICANIWILL',
          premble: 'Använd min kod: RICKARDB15 så får du 15% rabatt på träningskläder hos ICANIWILL',
          button: 'HANDLA NU',
          url: 'https://click.adrecord.com/?c=28930&p=886',
          color: 'cyan darken-1',
          btnColor: 'cyan darken-4'
        },
      ]
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

