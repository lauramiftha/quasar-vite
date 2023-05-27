<template>
  <q-layout view="lHh Lpr fFf">
    <q-header elevated class="bg-primary text-white" height-hint="98">
      <q-toolbar>
        <q-btn dense flat round icon="menu" @click="toggleLeftDrawer" />

        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" alt="Logo" />
          </q-avatar>
          Office Scheduler
        </q-toolbar-title>

        <q-btn dense flat round icon="settings" @click="toggleRightDrawer" />
      </q-toolbar>

      <q-tabs align="left">
        <q-route-tab to="/" label="Home" />
        <q-route-tab to="/about" label="About" />
        <q-route-tab to="/schedule" label="Schedule" />
        <q-route-tab to="/calendar" label="Calendar" />
        <q-route-tab to="/tasks" label="Tasks" />
      </q-tabs>
    </q-header>

    <q-drawer show-if-above v-model="leftDrawerOpen" side="left" bordered>
      <!-- Left drawer content -->
    </q-drawer>

    <q-drawer show-if-above v-model="rightDrawerOpen" side="right" bordered>
      <!-- Right drawer content -->
    </q-drawer>

    <q-page-container>
      <div class="q-ma-lg">
        <router-view />
      </div>
    </q-page-container>

    <q-footer elevated class="bg-grey-8 text-white">
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" alt="Logo" />
          </q-avatar>
          <div>Office Scheduler</div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script setup>
import { ref } from "vue";

const leftDrawerOpen = ref(false);
const rightDrawerOpen = ref(false);

const toggleLeftDrawer = () => {
  leftDrawerOpen.value = !leftDrawerOpen.value;
};

const toggleRightDrawer = () => {
  rightDrawerOpen.value = !rightDrawerOpen.value;
};
</script>

<style scoped>
.q-header {
  font-size: 16px;
}

.q-toolbar-title {
  font-size: 18px;
  font-weight: bold;
}

.q-tabs {
  padding-left: 20px;
}

.q-drawer {
  width: 300px;
  background-color: #f5f5f5;
}

.q-page-container {
  margin: 20px;
}

.q-footer {
  padding: 10px;
  text-align: center;
  font-size: 14px;
}

.q-toolbar-title div {
  margin-left: 10px;
}

.q-avatar img {
  max-width: 40px;
  max-height: 40px;
}
</style>
