<template>
  <div>
    <nuxt/>
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
  
  export default {
  
  }
</script>


<style>
@font-face {
font-family: 'Acherus Grotesque Regular';
font-style: normal;
font-weight: normal;
src: local('Acherus Grotesque Regular'), url('/assets/acherus_grotesque_-_regular.woff') format('woff');
}

html {
  /* font-family: "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; */
  font-family:'Acherus Grotesque Regular', "Source Sans Pro", -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*, *:before, *:after {
  box-sizing: border-box;
  margin: 0;
}
</style>

