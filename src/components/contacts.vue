<script setup>
import { ref } from 'vue'

defineProps({
  msg: String
})

const count = ref(0)
</script>  

<template>

  <div class="q-pa-md row inline" style="max-width: 350px"> 
    
    <q-list dense bordered padding class="rounded-borders" > 
      <div class="text-h6 text-center text-accent"> contact </div>

      <q-item 
            tag="a"
            clickable>
              <q-icon :color="$q.dark.isActive ? 'white' : 'accent'" name="call" size="sm" />
        <q-item-section >
          0769542411
        </q-item-section>
      </q-item>

      <q-item 
            tag="a"
            href="mailto:imene.sebai@etu.univ-lyon1.fr"
            clickable>
              <q-icon :color="$q.dark.isActive ? 'white' : 'accent'" name="mail" size="sm"/>
        <q-item-section>
          Adresse mail
        </q-item-section>
      </q-item>

      

      <q-item 
            tag="a"
            href="https://www.linkedin.com/in/imène-sebai-401973207/"
            clickable>
              <q-icon :color="$q.dark.isActive ? 'white' : 'accent'" name="fa-brands fa-linkedin-in" size="sm"/>
        <q-item-section>
          LinkedIn
        </q-item-section>
      </q-item>

    </q-list>
  </div>
</template>

<style> 

</style>