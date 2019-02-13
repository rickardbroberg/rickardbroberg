<template>
    <div>
      <vheader v-bind="header"/>
      
      <section flex row class="workouts">
        <article class="workout">
          <div></div>
          <h1>Title</h1>
          <p>premble</p>
        </article>
      </section>
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

<style scoped>
.workouts{
  
}
.workout{
  box-sizing: border-box;
  width: 280px;
  padding: 8px;
  border: 1px solid #000;
  box-shadow: 0 2px 2px #000;
}
</style>

