<template>
    <div>
      <vheader v-bind="header"/>
      
      <v-container
        grid-list-xl
      >
        <v-layout wrap>
          <v-flex xs12>

            <v-card>
              <v-img
                class="white--text"
                height="200px"
                src="https://cdn.vuetifyjs.com/images/cards/docks.jpg"
              >
                <v-container fill-height fluid>
                  <v-layout fill-height>
                    <v-flex xs12 align-end flexbox>
                      <span class="headline">Top 10 Australian beaches</span><br>
                      <span class="grey--text">Number 10</span><br>
                      <span>Whitehaven Beach</span><br>
                      <span>Whitsunday Island, Whitsunday Islands</span><br>
                      <v-btn flat color="orange">Share</v-btn>  
                    </v-flex>
                  </v-layout>
                </v-container>
              </v-img>
            </v-card>

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
        title: 'Mina träningstips',
        subheading: 'Hitta inspiration och tips till övrningar',
        image: 'traningstips.jpg'
      },
      items: [
        {
          title: 'OVER NIGHT OATS',
          premble: 'Letar du efter en fitnessfrukost? Här är min favorit baserad på proteinpulver och havregryn...',
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
          premble: 'Genom att använda min kod: RICKARDB15 får du 15% rabatt på träningskläder hos ICANIWILL',
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

