<template>
  <div>
    <vheader v-bind="header"/>
    <sidebar/>
    

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
        title: 'Rickard Broberg',
        subheading: 'Vem är jag',
        image: 'header.jpg'
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

