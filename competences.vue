<template>
    <div class=" my card row items-start justify-end q-gutter-lg ">
      <div class="col-8">
          <q-card class="my-card">
              <div class="row q-pa-lg">
                  <div class="col">
                  <div class="text-h5">Compétences Professionnelles</div>
                  </div>
                  <div class="col">
                  <div class="text-h5">Compétences Transversalles</div>
                  </div>
              </div>

              <div class="row justify-around q-pa-sm">
                  <div class="col-5">
                  <span class="text-h6">Informatiques <q-linear-progress rounded size="xl" :value="0.7" color="accent"/></span>
                  </div>
                  <div class="col-5">
                  <span class="text-h6">Anglais<q-linear-progress rounded size="xl" :value="0.75" color="accent"/></span>
                  </div>
              </div>

              <div class="row justify-around q-pa-sm">
                  <div class="col-5">
                  <span class="text-h6">Programmation <q-linear-progress rounded size="xl" :value="0.9" color="accent"/></span>
                  </div>
                  <div class="col-5">
                  <span class="text-h6">Espagnol<q-linear-progress rounded size="xl" :value="0.7" color="accent"/></span>
                  </div>
              </div>

              <div class="row justify-around q-pa-sm">
                  <div class="col-5">
                  <span class="text-h6">Coopérer au sein d’une équipe <q-linear-progress rounded size="xl" :value="1" color="accent"/></span>
                  </div>
                  <div class="col-5">
                  <span class="text-h6">Arabe<q-linear-progress rounded size="xl" :value="0.95" color="accent"/></span>
                  </div>
              </div>

              <div class="row justify-around q-pa-sm">
                  <div class="col-5">
                  <span class="text-h6">Développer des idées innovantes <q-linear-progress rounded size="xl" :value="0.99" color="accent"/></span>
                  </div>
                  <div class="col-5">
                  <span class="text-h6">Permis B<q-linear-progress rounded size="xl" :value="1" color="accent"/></span>
                  </div>
              </div>
          </q-card>
      </div>
    </div>
</template>

<style lang="sass" scoped>
.my-card 

  margin-right: 18px

</style>