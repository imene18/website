<template class="row inline">
  <q-layout view="lHh lpr lFf " container style="height: 50px">
    <q-header :class="$q.dark.isActive ? 'bg-dark text-white' : 'bg-white text-black'" reveal height-hint="200">
      <q-toolbar>
        <q-toolbar-title class="text-h4 justify-around">
          Mon <span :class="$q.dark.isActive ? 'text-accent text-weight-bold' : 'text-accent text-weight-bold'">CV</span>
        </q-toolbar-title>
      <q-btn @click="$q.dark.toggle()"  :icon="$q.dark.isActive ? 'nights_stay' : 'wb_sunny'" :color="$q.dark.isActive ? 'white' : 'black'" flat size="md"/>
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>


