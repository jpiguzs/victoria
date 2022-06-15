<template>
  <q-layout view="lHh Lpr lFf">
    <q-header class="bg-transparent">
      <q-toolbar class="bg-transparent">
               <img  src="~assets/logo.png" alt=""  style="width: 58px; height: 61px" srcset=""/>

        <q-toolbar-title>
 
        </q-toolbar-title>

        <div></div>
      </q-toolbar>
    </q-header>

   

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>
import { defineComponent, ref } from 'vue'




export default defineComponent({
  name: 'MainLayout',

  components: {
    
  },

  setup () {
    const leftDrawerOpen = ref(false)

    return {
  
      leftDrawerOpen,
      toggleLeftDrawer () {
        leftDrawerOpen.value = !leftDrawerOpen.value
      }
    }
  }
})
</script>
