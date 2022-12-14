<template>
<div class="q-pa-md">
<q-toolbar class="text-white rounded-borders justify-center" style="background: radial-gradient(circle, #a36ca3 0%, #a36ca3 100%)"></q-toolbar></div>
  <div class="q-pa-md q-gutter-sm">
    <q-tree
      :nodes="customize"
      node-key="label"
      default-expand-all
    >

      <template v-slot:default-header="prop">
        <div class="row items-center text-h6">
          <q-icon :name="prop.node.icon || 'share'" color="accent" size="28px" class="q-mr-sm" />
          <div class="text-weight-bold text-wight">{{ prop.node.label }}</div>
        </div>
      </template>

      <template v-slot:default-body="prop">
        <div v-if="prop.node.story">
          <span class="text-weight-bold"></span> {{ prop.node.story }}
        </div>
        <span v-else class="text-weight-light text-black"></span>
      </template>
    </q-tree>
  </div>
<div class="q-pa-md">
<q-toolbar class="text-white rounded-borders justify-center" style="background: radial-gradient(circle, #a36ca3 0%, #a36ca3 100%)"></q-toolbar></div>
</template>

<script>
import { ref } from 'vue'

const count = ref(0)
export default {
  setup () {
    return {
      customize: [
        {
          label: 'Formations',
          icon: 'school',
          header: 'root',
          children: [
            {
              label: 'Licence Science pour la Santé spécialité Objets Connectés Université Claude Bernard Lyon 1 / 2020-2023',
              icon: 'settings_input_antenna',
              header: 'generic',
              children: [
                {
                  label: 'UE Informatique et réseau appliquée à la santé',
                  header: 'generic',
                  body: 'story',
                  story: 'programmation (logiciel pour doser l’insuline, principe de l’échographe, web, Javascript, Vue), modélisation en UML, SQL'
                },
                {
                  label: 'UE Data Science',
                  body: 'story',
                  story: 'manipulation, prédiction, analyse de données, réseaux de neurones'
                },
                {
                  label: 'UE Mathématiques et statistiques appliquées à la santé',
                  body: 'story',
                },
                {
                  label: 'UE Développement et maintenance des dispositifs médicaux',
                  body: 'story',
                },
                {
                  label: 'UE Neurosciences',
                  body: 'story',
                },
                {
                  label: 'UE Outils diagnostiques et physiopathologiques',
                  body: 'story',
                },
              ]
            },
            {
              label: 'Première année communes aux études de santé Université Claude Bernard Lyon 1 / 2019-2020',
              header: 'generic',
              body: 'toggle',
              caption: 'Why are we as consumers so captivated by stories of great customer service? Perhaps it is because...',
              enabled: false,
              icon: 'medical_services',
            
            },
            {
              label: 'Baccalauréat Scientifique Lycée Parc Chabrières Oullins / 2019',
              icon: 'workspace_premium',
              
            }
          ]
        }
      ]
    }
  }
}
</script>
