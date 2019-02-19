<template>
  <div>
  
  <v-sidebar />
  
   <div id="hero">
        <video playsinline autoplay muted loop poster="/placeholder.png" id="bgvideo" width="100%">
            <source src="/abs-ball-deluxe.mp4" type="video/mp4">
        </video>
    </div>
    <v-container grid-list-md text-xs-center fill-height>
        <v-layout row wrap>  
          
          
          <v-flex hero-text xs12 align-self-center>
            <h1>Rickard Broberg</h1>
            <h2>A mens physique fitness athlete</h2>
          </v-flex>
        

          <v-flex v-for="item in frontboxes" :key="`4${item}`" xs12 sm12 md4>
              <v-card :color="item.color">
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
  </div>
</template>


<script>
import VSidebar from '~/components/VSidebar.vue'

export default {
  data: () => ({ 
    frontboxes: [
        {
            title: 'OVER NIGHT OATS',
            premble: 'Letar du efter en fitnessfrukost? Denna är baserad på proteinpulver och havregryn...',
            button: 'Läs receptet',
            url: 'kostrad/overnight-oat-with-proteinpowder',
            color: 'grey lighten-2',
            btnColor: 'grey lighten-1'
        },
        {
            title: 'LÄR DIG GÖRA CHINS',
            premble: 'Här får du mina bästa tips för att lära dig göra chins eller pullups...',
            button: 'Läs mina tips',
            url: 'traningstips/chins-pullups',
            color: 'grey lighten-2',
            btnColor: 'grey lighten-1'
        },
        {
            title: 'ICANIWILL',
            premble: 'Använd min kod: RICKARDB15 så får du 15% rabatt på träningskläder hos ICANIWILL',
            button: 'HANDLA NU',
            url: 'https://click.adrecord.com/?c=28930&p=886',
            color: 'grey lighten-2',
            btnColor: 'grey lighten-1'
        },
    ],
  }),
  components: {
    VSidebar
  }


}
</script>

<style>
#hero{
    position: absolute;
    top: 64px;
    left: 0;
    height: 500px;
    width: 100%;
    overflow: hidden;
    z-index: -100;
}
video#bgvideo {
    position: fixed;
    top: 50%;
    left: 50%;
    min-width: 100%;
    min-height: 100%;
    width: auto;
    height: auto;
    z-index: -100;
    -ms-transform: translateX(-50%) translateY(-50%);
    -moz-transform: translateX(-50%) translateY(-50%);
    -webkit-transform: translateX(-50%) translateY(-50%);
    transform: translateX(-50%) translateY(-50%);
    background: url(/placeholder.png) no-repeat;
    background-size: cover;
}

.hero-text{
    margin: 28% 0 20% 0;
}

.hero-text h1{
    font-size: 4.57143rem;
    line-height: 5.14286rem;
    letter-spacing: -.01429rem;
    word-break: initial;
    font-family:'Acherus Grotesque Regular';
    color:#ffffff;

}
.hero-text h2{
    font-size: 1.6rem;
    font-weight: 400;
    font-family:'Acherus Grotesque Regular';
    color:#ffffff;
}
</style>
