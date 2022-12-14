<template>

<div class="q-pa-md">

<div class="offset-1 col-3 column justify-around">

<q-toolbar class="text-white rounded-borders justify-end" style="background: radial-gradient(circle, #a36ca3 0%, #a36ca3 100%)">

<q-btn-dropdown  label="informations complémentaires" style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)">
<q-list>
<div class="q-pa-md q-gutter-sm justify-around ">
<q-btn href="https://docs.google.com/document/d/1oYr00EClRYI69fk3PJwtdiIqZl3AAxqC/edit" target="_blank" label="Voir ma lettre de motivation" style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)" />
</div>
</q-list>

<q-list>
<div class="q-pa-md q-gutter-sm justify-around ">
<q-btn href="Imène SEBAI pdf.pdf" target="_blank" label="Télécharger mon CV en PDF" style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)" />
</div>
</q-list>
</q-btn-dropdown>


</q-toolbar>

</div>

</div>

<div class="row inline"> 
        <div class="q-pa-md row items-start">
        <q-card class="my-card q-pa-xs row inline">
        <q-img src="IMG_5132 Small.jpeg">
        <div class="absolute-bottom">
        <div class="text-center">Imène SEBAI</div>
        <div class=" text-center">18/02/2001</div>
        </div>
        </q-img>


        <q-card-actions>

          <div class=" row inline"> 
            
            <q-list dense > 
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
        </q-card-actions>

        </q-card>

        </div>

        <div class="row inline col-10 column q-pa-md">

            <q-card 
              style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%); width:100%; "
            >
              <q-card-section>
                <div heading class="q-pa-md text-h4 text-center ">Recherche de stage </div>
                <div class="text-subtitle1">Du 17 avril au 9 juin 2023</div>
              </q-card-section>

              <q-card-section class="q-pt-none text-subtitle1">
                {{ lorem }}

              </q-card-section>
            </q-card>

          </div>
</div>
</template>


<script>
import { ref } from 'vue'

export default {
  props: {
  },
  setup () {
    return {
      lorem: "Je suis en troisième année de licence Science pour la Santé. Etant très intéressée par l'intelligence artificielle, l'innovation thérapeuthique, la neuroscience et l'informatique, je souhaiterais réaliser un stage au sein de votre strat up afin d’enrichir mon expérience et de vous apporter mon savoir et ma créativité."
    }
  }
}
</script>



