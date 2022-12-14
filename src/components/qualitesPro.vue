<template>
<div class="q-pa-md">
<div class="offset-1 col-3 column justify-between">
 <q-toolbar class="text-white rounded-borders justify-center" style="background: radial-gradient(circle, #a36ca3 0%, #a36ca3 100%)">
    <div class="items-start q-gutter-md ">
      <q-btn-dropdown label="Qualités professionnelles" style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)" @click="layout = true" />

      <q-dialog v-model="layout" >
        <q-layout view="Lhh lpR fff" container class="bg-white">
          <q-header style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)">
            <q-toolbar>
              <q-toolbar-title>Qualités professionnelles</q-toolbar-title>
              <q-btn flat v-close-popup round dense icon="close" />
            </q-toolbar>
          </q-header>

          <q-page-container :class="$q.dark.isActive ? 'bg-dark text-white' : 'bg-white text-black'">
            <q-page padding>
              <p v-for="n in contentSize" :key="n">
                {{ lorem1 }}
              </p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem2 }}</p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem3 }}</p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem4 }}</p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem5 }}</p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem6 }}</p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem7 }}</p>
              <p v-for="n in contentSize" :key="n">
                {{ lorem8 }}</p>
            </q-page>
          </q-page-container>
        </q-layout>
      </q-dialog>
    </div>
  </q-toolbar>
</div>
</div>
</template>

<script>
import { ref, computed } from 'vue'

export default {
  setup () {
    const moreContent = ref(true)

    return {
      layout: ref(false),

      moreContent,
      contentSize: computed(() => moreContent.value ? 1 : 1),

      lorem1: "Capacité d'adaptation",
      lorem2: "Travail en équipe",
      lorem3: "Autonome",
      lorem4: "Curieuse",
      lorem5: "Sens de l'organisation",
      lorem6: "Rigoureuse",
      lorem7: "Dynamique et motivée",
      lorem8: 'Nettoyage des locaux'
    }
  }
}
</script>
