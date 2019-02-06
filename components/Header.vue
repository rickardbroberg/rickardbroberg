<template>
  <div class="head">
    <v-toolbar>
        <v-toolbar-side-icon></v-toolbar-side-icon>
        <v-toolbar-title>Rickard Broberg - Fitness Athlete</v-toolbar-title>
        <v-spacer></v-spacer>
        <v-toolbar-items class="hidden-sm-and-down">
        <v-btn flat>Träningstips</v-btn>
        <v-btn flat>Kost</v-btn>
        <v-btn flat>Instagram</v-btn>
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
