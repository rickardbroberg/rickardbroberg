<template>
  <section class="container">
    <div>
      <header/>
      <app-logo/>
    </div>
  </section>
</template>

<script>
import Vue from 'vue'
import Vuetify from 'vuetify'

Vue.use(Vuetify)

import AppLogo from '~/components/AppLogo.vue'
import Header from '~/components/Header.vue'

export default {
  components: {
    AppLogo,
    Header
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

