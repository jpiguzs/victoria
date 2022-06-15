<template>
  <div>
     <div class="q-pa-md">
    <q-carousel
      arrows
      animated
      v-model="slide"
      height="400px"
      control-color="btn-slider"

         control-type="regular"
          v-model:fullscreen="fullscreen"
      infinite
    >
      <q-carousel-slide name="first" img-src="https://cdn.quasar.dev/img/mountains.jpg">
        <div class=" custom-caption text-center">
          <div class="title-v">¿Que ofrecemos?</div>
          <div class="subtitle-v ">¡Exelencia académica en las mejores instalaciones!</div>

        </div>
        <div class="btn--slider">
            <q-btn class="btn--blue1 btn--vic" label="Ver mas" @click="setImgToModal('https://cdn.quasar.dev/img/mountains.jpg')">

            </q-btn>
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="second" img-src="https://cdn.quasar.dev/img/parallax1.jpg">
        <div class=" custom-caption">
          <div class="text-h2">Second stop</div>
          <div class="text-subtitle1">Famous City</div>
        </div>
        <div class="btn--slider">
            <q-btn class="btb--blue1" label="Ver mas">

            </q-btn>
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="third" img-src="https://cdn.quasar.dev/img/parallax2.jpg">
        <div class=" custom-caption">
          <div class="text-h2">Third stop</div>
          <div class="text-subtitle1">Famous Bridge</div>
        </div>
      </q-carousel-slide>
      <template v-slot:control>
        <q-carousel-control
          position="bottom-right"
          :offset="[18, 18]"
        >
          <q-btn
            push round dense color="white" text-color="primary"
            :icon="fullscreen ? 'fullscreen_exit' : 'fullscreen'"
            @click="fullscreen = !fullscreen"
          />
        </q-carousel-control>
      </template>
    </q-carousel>
  </div>
  <q-dialog
        v-model="showModal"
        persistent
        :maximized="maximizedToggle"
        transition-show="slide-up"
        transition-hide="slide-down"

  >
      <q-card>
        <q-bar>
          <q-space />

          <q-btn dense flat icon="minimize" @click="maximizedToggle = false" :disable="!maximizedToggle">
            <q-tooltip v-if="maximizedToggle" class="bg-white text-primary">Minimize</q-tooltip>
          </q-btn>
          <q-btn dense flat icon="crop_square" @click="maximizedToggle = true" :disable="maximizedToggle">
            <q-tooltip v-if="!maximizedToggle" class="bg-white text-primary">Maximize</q-tooltip>
          </q-btn>
          <q-btn dense flat icon="close" v-close-popup>
            <q-tooltip class="bg-white text-primary">Close</q-tooltip>
          </q-btn>
        </q-bar>
        <img :src="selectImg" style="width:100%; height:100%">
      </q-card>
  </q-dialog>
  </div>
</template>

<script>
import { ref } from 'vue'
export default {
   name: 'Slider-vue',
  setup () {
    const showModal = ref(false);
    const selectImg = ref(null);
    const setImgToModal= (img)=>{
      selectImg.value = img;
      showModal.value = true;
    }
    return {
      slide: ref('first'),
      maximizedToggle: ref(true),
      showModal,
      selectImg,
      setImgToModal,
       fullscreen: ref(false)
    }
  }
}
</script>
