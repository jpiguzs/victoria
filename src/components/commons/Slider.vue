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
      <q-carousel-slide name="first" img-src="/queOfrecemos.jpg">
        <div class=" custom-caption text-center">
          <div class="title-v">¿Que ofrecemos?</div>
          <div class="subtitle-v ">¡Excelencia académica en las mejores instalaciones!</div>

        </div>
        <div class="btn--slider">
           

          
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="Dos" img-src="/formacion.jpg">
        <div class=" custom-caption text-center">
          <div class="title-v">Formación Integral</div>
          <div class="subtitle-v "></div>

        </div>
        <div class="btn--slider">
           

          
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="tres" img-src="/docentes.jpg">
        <div class=" custom-caption text-center">
          <div class="title-v">Docentes Comprometidos</div>
          <div class="subtitle-v "></div>

        </div>
        <div class="btn--slider">
           

          
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="second" img-src="/basico.jpg">
        <div class=" custom-caption">
          <div class="title-v">Educación Básica</div>
          
        </div>
        <div class="btn--slider">
            
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="third" img-src="/media3.jpg">
        <div class=" custom-caption">
          <div class="title-v text-center">Educación Media General</div>
          <div class="subtitle-v  text-center">Primer nivel</div>
          
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="four" img-src="/diversificado.jpg">
        <div class=" custom-caption">
          <div class="title-v">Educación Media General</div>
          <div class="subtitle-v text-center">Segundo nivel</div>
          
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="five" img-src="/cancha.jpg">
        <div class=" custom-caption">
          <div class="title-v">Area Deportiva</div>
          
          
        </div>
      </q-carousel-slide>
       <q-carousel-slide name="six" img-src="/laboratorio.jpg">
        <div class=" custom-caption">
          <div class="title-v">Laboratorio de Computaciòn</div>
          
          
        </div>
      </q-carousel-slide>
        <q-carousel-slide name="seven" img-src="/quimica.jpg">
        <div class=" custom-caption">
          <div class="title-v">Laboratorio de Química</div>
          
          
        </div>
      </q-carousel-slide>
      <q-carousel-slide name="ocho" img-src="/fachada.jpg">
        <div class=" custom-caption">
          <div class="title-v">Conocénos</div>
          
          
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
