<script>
// This starter template is using Vue 3 <script setup> SFCs
// Check out https://vuejs.org/api/sfc-script-setup.html#script-setup
import layout from './layout.vue'
import experiences from './components/experiences.vue'
import centredinterets from './components/centredinterets.vue'
import qualitesPro from './components/qualitesPro.vue'
import aboutme from './components/aboutme.vue'
import image from "/Users/imenesebai/vite-project/IMG_5132 Small.jpeg"
import { useQuasar } from 'quasar'
import competences from './components/competences.vue'
import formation from './components/formation.vue'


export default {
  props: {
  },
  methods: {
  },
  components: {
    layout,
    aboutme,
    image,
    centredinterets,
    experiences,
    qualitesPro,
    competences,
    formation,
  },
  setup () {
    const $q = useQuasar()

    // calling here; equivalent to when component is created
    $q.dark.set(false)
  }
}
</script>

<template>
  <div >
    <layout msg="CV Imène SEBAI"/>
    <aboutme msg="CV Imène SEBAI"/>
    <experiences msg="CV Imène SEBAI"/>
    <formation msg="CV Imène SEBAI"/>
    <competences msg="CV Imène SEBAI"/>
    <centredinterets msg="CV Imène SEBAI"/>
    <qualitesPro msg="CV Imène SEBAI"/>


</div> 
</template>