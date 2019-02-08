<template>
  <div class="head">
  <v-navigation-drawer
      :clipped="drawer.clipped"
      :fixed="drawer.fixed"
      v-model="drawer.open"
      app
      dark
    >
      <v-list>
        <v-list-tile
        v-for="item in items"
        :key="item.title"
        :href="item.url"
      >
        <v-list-tile-action>
          <v-icon>{{ item.icon }}</v-icon>
        </v-list-tile-action>
        <v-list-tile-content>
          <v-list-tile-title>{{ item.title }}</v-list-tile-title>
        </v-list-tile-content>
      </v-list-tile>
      </v-list>
    </v-navigation-drawer>
    
    <v-toolbar
      app
      dark
      color="grey darken-4"
      :fixed="toolbar.fixed"
      :clipped-left="toolbar.clippedLeft"
    >
      <v-toolbar-side-icon 
        @click.stop="toggleDrawer"
      ></v-toolbar-side-icon>
        <v-toolbar-title>Rickard Broberg</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
        <v-btn href="/" flat>
            <v-icon>fa-home</v-icon>
        </v-btn>
        <v-btn href="traningstips" flat>Träningstips</v-btn>
        <v-btn href="kostrad" flat>Kostråd</v-btn>
        <v-btn href="https://www.instagram.com/rickardbroberg" flat>
          <v-icon>fa-instagram</v-icon>
        </v-btn>
        </v-toolbar-items>
    </v-toolbar>
   <div id="hero">
        <video playsinline autoplay muted loop poster="/placeholder.png" id="bgvideo" width="100%">
            <source src="/abs-ball-deluxe.mp4" type="video/mp4">
        </video>
    </div>
    <div class="large-push">
        <h1 style="text-align: left;">Rickard Broberg</h1>
        <h2>A mens physique fitness athlete</h2>
    </div>
  </div>
</template>


<script>
export default {
  data: () => ({
    items: [
      { title: 'Start', icon: 'fa-home', url: '/' },
      { title: 'Träningstips', icon: 'fa-bomb', url: 'traningstips' },
      { title: 'Kostråd', icon: 'fa-cutlery', url: 'kostrad' },
      { title: 'Bio', icon: 'fa-cube', url: 'om' },
      { title: 'Instagram', icon: 'fa-instagram', url: 'https://www.instagram.com/rickardbroberg' },
    ],  
    drawer: {
      open: false,
      clipped: true,
      fixed: true
    },
    toolbar: {
      fixed: true,
      clippedLeft: true
    }
  }),
  methods: {
    toggleDrawer () {
        this.drawer.open = !this.drawer.open
    }
  }

}
</script>

<style>

@font-face {
font-family: 'Acherus Grotesque Regular';
font-style: normal;
font-weight: normal;
src: local('Acherus Grotesque Regular'), url('/assets/acherus_grotesque_-_regular.woff') format('woff');
}

body{
  background-color:#212121;
  color:#eeeded;
}
#hero{
    position: absolute;
    top: 0;
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
.large-push{
    position: absolute;
    left: 12%;
    width: 50%;
    top:50%;
    z-index: 9999;
    opacity: 0.5;
}
.large-push h1{
    font-size: 4.57143rem;
    line-height: 5.14286rem;
    letter-spacing: -.01429rem;
    word-break: initial;
    font-family:'Acherus Grotesque Regular';
}
.large-push h2{
    font-size: 1.6rem;
    font-weight: 400;
    font-family:'Acherus Grotesque Regular';
}
</style>
