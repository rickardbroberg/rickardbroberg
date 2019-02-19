<template>
  <div>
    
    <v-sidebar />
    
  </div>
</template>


<script>
import VSidebar from '~/components/VSidebar.vue'

export default {
  data: () => ({
    
  }),
  props: ['image', 'title', 'subheading'],
  components: {
    VSidebar
  }
}
</script>

<style>

</style>
