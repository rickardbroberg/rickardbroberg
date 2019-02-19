<template>
    <div>
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
    </div>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: 'Start', icon: 'fa-home', url: '/' },
      { title: 'Träningstips', icon: 'fa-gears', url: 'traningstips' },
      { title: 'Kostråd', icon: 'fa-cutlery', url: 'kostrad' },
      { title: 'Modelljobb', icon: 'fa-user-o', url: 'modelljobb' },
      { title: 'Tävlingar', icon: 'fa-trophy', url: 'tavlingar' },
      { title: 'Samarbeten', icon: 'fa-check-square-o', url: 'samarbeten' },
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
  },
 
}
</script>

<style>

</style>
