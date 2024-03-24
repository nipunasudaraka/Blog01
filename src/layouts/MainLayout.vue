<template>
  <q-layout view="lHh Lpr lFf" class="no-padding">
    <div class="q-pa-md no-padding">
      <q-toolbar class="bg-red text-white shadow-2">
        <q-space />

        <router-link to="/">
          <q-btn stretch flat label="home" class="text-white" />
        </router-link>

        <router-link to="/about">
          <q-btn stretch flat label="About" class="text-white" />
        </router-link>

        <router-link to="/blog">
          <q-btn stretch flat label="Bolg" class="text-white" />
        </router-link>
      </q-toolbar>
    </div>
    <q-page-container>
      <router-view />
    </q-page-container>
    <!-- Footer -->
    <q-toolbar class="bg-red text-white full-height q-mt-md">
      <q-space />
      <router-link to="/">
        <q-btn flat dense round icon="home" class="text-white q-mr-xs" />
      </router-link>
      <router-link to="/about">
        <q-btn flat dense round icon="info" class="text-white q-mr-xs" />
      </router-link>
      <router-link to="/blog">
        <q-btn flat dense round icon="edit" class="text-white q-mr-xs" />
      </router-link>
      <q-space />
      <q-icon name="facebook" size="md" class="text-white q-mr-xs" />
      <q-icon name="twitter" size="md" class="text-white q-mr-xs" />
      <q-icon name="instagram" size="md" class="text-white q-mr-xs" />
      <q-icon name="linkedin" size="md" class="text-white q-mr-xs" />
      <q-space />
    </q-toolbar>
  </q-layout>
</template>

<script setup></script>
