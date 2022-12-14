<template>
  <div class="my-card justify-around">
    <q-card class="text-center text-h6" style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)">Centre d'intérêt

    <q-carousel
      style="background: radial-gradient(circle, #dcbce0 0%, #c88cd1 100%)"
      v-model="slide"
      transition-prev="scale"
      transition-next="scale"
      swipeable
      animated
      control-color="white"
      navigation
      padding
      arrows
      height="200px"
      class="text-white shadow-1 rounded-borders" 
    >
      <template v-slot:navigation-icon="{ active, btnProps, onClick }"> 
        <q-btn v-if="active" size="lg" icon="home" color=" accent" flat round dense @click="onClick" />
        <q-btn v-else size="sm" :icon="btnProps.icon" color="white" flat round dense @click="onClick" />
      </template>
      <q-carousel-slide name="food_bank" class="column no-wrap flex-center">
        <q-icon name="food_bank" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem1 }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="travel_explore" class="column no-wrap flex-center">
        <q-icon name="travel_explore" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem2 }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="shopping_bag" class="column no-wrap flex-center">
        <q-icon name="shopping_bag" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem3 }}
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="sports_tennis" class="column no-wrap flex-center">
        <q-icon name="sports_tennis" size="56px" />
        <div class="q-mt-md text-center">
          {{ lorem4 }}
        </div>
      </q-carousel-slide>
    </q-carousel>
    </q-card>
  </div>
</template>

<script>
import { ref } from 'vue'

export default {
  setup () {
    return {
      slide: ref('style'),
      lorem1: 'Cuisiner',
      lorem2: 'Voyager',
      lorem3: 'Shopping et mode',
      lorem4: 'Sport'

    }
  }
}
</script>

<style lang="sass" scoped>
.my-card 
  max-width: 390px
  margin-left: 17px
  margin-right: 10px
  margin-top: -230px


</style>