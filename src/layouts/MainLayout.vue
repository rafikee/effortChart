<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <q-toolbar-title>VCU Effort Chart</q-toolbar-title>

        <div>Effort Chart 0.1</div>
      </q-toolbar>
      <q-tabs v-model="tab" align="left">
        <q-tab name="charts" label="Charts" />
        <q-tab name="players" label="Players" />
        <q-tab name="settings" label="Settings" />
      </q-tabs>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from "vue";

export default defineComponent({
  name: "MainLayout",

  components: {},

  setup() {
    const leftDrawerOpen = ref(false);

    return {};
  },
});
</script>
