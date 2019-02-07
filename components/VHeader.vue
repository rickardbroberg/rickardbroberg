<template>
  <div class="head">
    <v-toolbar>
        <v-toolbar-side-icon></v-toolbar-side-icon>
        <v-toolbar-title>{{ pageTitle }}</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
        <v-btn href="/" flat>
            <v-icon>home</v-icon>
        </v-btn>
        <v-btn href="traningstips" flat>Träningstips</v-btn>
        <v-btn href="kost" flat>Kost</v-btn>
        <v-btn href="https://www.instagram.com/rickardbroberg" flat>Instagram</v-btn>
        </v-toolbar-items>
    </v-toolbar>
    <v-parallax src="https://cdn.vuetifyjs.com/images/parallax/material.jpg"></v-parallax>
  </div>
</template>

<style>
.head {
  float:left;
  height: 580px;
  width: 100%;
}
</style>
