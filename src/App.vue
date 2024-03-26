<script setup lang="ts">
import { RouterLink, RouterView } from 'vue-router'
</script>

<template>
  <v-app>
    <v-layout>
      <v-app-bar :elevation="1">
        <template v-slot:prepend>
          <v-app-bar-nav-icon></v-app-bar-nav-icon>
        </template>
        <v-app-bar-title>ToueRe</v-app-bar-title>
        <template v-slot:append>
          <v-btn icon="mdi-heart"></v-btn>
          <v-btn icon="mdi-magnify"></v-btn>
          <v-btn icon="mdi-dots-vertical"></v-btn>
        </template>
      </v-app-bar>
      <v-navigation-drawer expand-on-hover rail>
        <v-list>
          <v-list-item
            prepend-avatar="https://randomuser.me/api/portraits/women/85.jpg"
            subtitle="sandra_a88@gmailcom"
            title="Sandra Adams"
          ></v-list-item>
        </v-list>
        <v-divider></v-divider>
        <v-list density="compact" nav>
          <v-list-item
            href="/"
            prepend-icon="mdi-folder"
            title="My Classroom"
            value="myfiles"
          ></v-list-item>
          <v-list-item
            href="/enrollment"
            prepend-icon="mdi-account-multiple"
            title="Enrollment"
            value="shared"
          ></v-list-item>
          <v-list-item
            href="/reports"
            prepend-icon="mdi-star"
            title="Sent Reports"
            value="starred"
          ></v-list-item>
        </v-list>
      </v-navigation-drawer>
      <RouterView />
    </v-layout>
  </v-app>
</template>

<style scoped></style>
