<template>
  <div>
    <q-card class=" card--info  text-white" :style="getStyle()">
      <div class="bg--info  ">
        <div >
          <div class="flex flex-center img--info">
            <img :src="icon" style="width: 75px;
height: 75px;" alt="" srcset="">
          </div>
          <div class=" flex flex-center  img--info">
            <q-btn :class="btnClass" class=" btn--vic" :label="title" @click="showModal=!showModal"></q-btn>
          </div>

        </div>
      </div>
    </q-card>
    <q-dialog v-model="showModal"

     transition-show="slide-up"
      transition-hide="slide-down"
    >
    <q-card :class="cardClass">
      <div class="row">
        <div class=" col-10 q-pa-sm row">
          <div class="col-6">
                 <img :src="icon" style="width: 75px;
                  height: 75px;" alt="" srcset="">
          </div>
          <div class="col-2 q-pt-md text-center text-white text--bold  text-h4">
              {{title}}
          </div>

        </div>

          <q-space />
    <div class="col-2" v-if="$q.platform.is.mobile" >
      <q-btn icon="cancel" class="text-white btn--close" dense  flat v-close-popup></q-btn>
    </div>
          <q-btn v-if="!$q.platform.is.mobile"  icon="cancel" class="text-white btn--close" dense  flat v-close-popup></q-btn>

        </div>
        <q-card-section class="text-white text-justify text-data">
          <slot></slot>













        </q-card-section>

    </q-card>

    </q-dialog>
  </div>
</template>

<script>
import { ref } from 'vue'

import { useQuasar } from 'quasar'
export default {
  // name: 'ComponentName',
  props:['title', 'icon', 'background', 'btnClass', 'cardClass', 'left'],
  setup () {
    return {
      showModal:ref(false),
      $q: useQuasar()
    }
  },
  methods:{
    getStyle(){
      return "background:url('"+this.background+"'); background-position:center"+(this.left ? 'left':'')
    }
  }
}
</script>
