<template>
  <div class="head">
    <v-toolbar dark>
        <v-toolbar-side-icon></v-toolbar-side-icon>
        <v-toolbar-title>{{ pageTitle }}</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
        <v-btn href="/" flat>
            <v-icon>home</v-icon>
        </v-btn>
        <v-btn href="traningstips" flat>Träningstips</v-btn>
        <v-btn href="kost" flat>Kost</v-btn>
        <v-btn href="https://www.instagram.com/rickardbroberg" flat>
          <v-icon>home</v-icon>
        </v-btn>
        </v-toolbar-items>
    </v-toolbar>
    <v-parallax dark height="350" :src="image">
      <v-layout
      align-center
      column
      justify-center
    >
      <h1 class="display-2 font-weight-thin mb-3">{{ title }}</h1>
      <h4 class="subheading">{{ subheading }}</h4>
    </v-layout>
    </v-parallax>
  </div>
</template>


<script>
export default {
  props: ['image', 'title', 'subheading']
}
</script>

<style>
body{
  background-color:#1b1b1b;
  color:#eeeded;
}
.head {
  float:left;
  width: 100%;
}
</style>
