<template>
  <v-card>
    <v-layout>
      <v-app-bar elevation="0" app color="light-blue-lighten-5" style="z-index: 100;">

        <template v-slot:prepend>
          <v-app-bar-nav-icon></v-app-bar-nav-icon>
        </template>

        <v-spacer></v-spacer>

        <v-btn icon>
          <v-icon>mdi-bell-outline</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-chat-outline</v-icon>
        </v-btn>

        <v-btn icon>
          <v-icon>mdi-account-outline</v-icon>
        </v-btn>
      </v-app-bar>

      <v-navigation-drawer app class="bg-blue">
        <v-list color="transparent">
          <v-list-item prepend-icon="mdi-view-dashboard" title="Dashboard"></v-list-item>
          <v-list-item prepend-icon="mdi-account-box" title="Account"></v-list-item>
          <v-list-item prepend-icon="mdi-gavel" title="Admin"></v-list-item>
        </v-list>

      </v-navigation-drawer>
    </v-layout>
  </v-card>
</template>