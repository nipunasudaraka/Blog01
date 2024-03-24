<template>
  <q-layout view="lHh Lpr lFf" class="no-padding">
    <div class="q-pa-md no-padding">
      <q-toolbar class="bg-red text-white shadow-2">
        <q-space />

        <q-separator dark vertical />
        <q-btn stretch flat label="About" />
        <q-separator dark vertical />
        <q-btn stretch flat label="Blog" />
      </q-toolbar>
    </div>
    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script setup></script>
