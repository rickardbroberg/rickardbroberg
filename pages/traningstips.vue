<template>
  <section class="">
    <div>
      <vheader v-bind="header"/>
      <section class="container">

      </section>
      <vfooter/>
    </div>
  </section>
</template>

<script>
import Vue from 'vue'
import Vuetify from 'vuetify'

Vue.use(Vuetify)

import 'vuetify/dist/vuetify.min.css'

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
  justify-content: center;
  align-items: center;
  text-align: center;
}

</style>

