 <script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>  

<template>
<div class="q-pa-md">
<q-toolbar class="text-white rounded-borders justify-center" style="background: radial-gradient(circle, #a36ca3 0%, #a36ca3 100%)"></q-toolbar></div>
  <div class="q-pa-lg row  justify-center">

    <q-card class="my-card">
      <q-card-section>
        <q-timeline :layout="layout" :side="side" color="secondary">
          <q-timeline-entry heading class="text-center">Expérience professionnelles</q-timeline-entry>

          <q-timeline-entry
            title="Stagiaire au centre de recherche en neuroscience de Lyon"
            subtitle="Au groupement hospitalie Est, à Bron, en mai 2022"
            side="right"
            color="purple"
            icon="psychology_alt"
          >
            <div>
              Chercheuse en neuroscience sur le coma et la conscience chez les patients cérébrolésés.
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Stagiaire chez Cuspide, Laboratoire de prothèse dentaire"
            subtitle="A Oullins, de mai à juin 2021"
            side="right"
            color="purple"
            icon="lan"
          >
            <div>
              Réalisation des prothèses dentaires par technique traditionnelle (manuelle) et par conception et fabrication assisté par ordinateur.
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Cours particulier"
            subtitle="A domicile, Régulièrement depuis 2020"
            side="left"
            icon="local_library"
            color="purple"
            avatar="https://cdn.quasar.dev/img/avatar3.jpg"
          >
            <div>
              Aide aux devoirs et soutien scolaire pour les collegiens.
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Agent d'entretien"
            subtitle="A lyon, emploi saisonnier depuis 2020"
            side="right"
            color="purple"
            icon="cleaning_services"
          >
            <div>
              Employée pour des agences de nettoyage : Atalian et GSF
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Garde d'enfant"
            subtitle="A domicile, occasionnellement depuis 2017"
            side="left"
            color="purple"
            icon="escalator_warning"

          >
            <div>
              Prise de repas, douche/toilette, temps de jeux, veille et surveillance jusqu'au retour des parents, respect des heures de coucher.
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Entretien de batiment"
            subtitle="Mairie de Pierre-Bénite, en juillet 2019"
            side="right"
            color="purple"
            icon="location_city"
          >
            <div>
              Entretien des écoles élémentaires de la ville.
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Stage de découverte 3ème Collège"
            subtitle="Crèche de Pierre-Bénite, 2015"
            side="right"
            color="purple"
            icon="child_care"
          >
            <div>
              Activité avec les enfants, prise de repas.
            </div>
          </q-timeline-entry>

          <q-timeline-entry
            title="Projet santé"
            subtitle="Graine de vie, centre social de Pierre-Bénite, 2014-2016"
            side="left"
            color="purple"
            icon="blind"
          >
            <div>
              Accompagnement des personnes âgées (sorties, loisirs...)
              visite de l'OMS, L'ONU, la Croix Rouge à Genève
              Réalisation d'un court métrage
            </div>
          </q-timeline-entry>
        </q-timeline>
      </q-card-section>
    </q-card>
  </div>
</template>

<style lang="sass" scoped>
.my-card
  width: 100%
</style>