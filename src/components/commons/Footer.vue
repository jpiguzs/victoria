<template>
  <div class="footer-v full-width q-pa-md">
      <div class="row">
        <div class="col-md-4 col-xs-6 col-sm-6">
          <div class="text--bold text-white row text--new">
             <img src="Marker.svg" style="width:24px" alt="" srcset=""> <span class="q-pl-sm" >Dirección:</span>

          </div>
          <div class="text-white row text--new">
              Edificio moderno nº 262. Av bolivar.
              Municipio Sotillo. Puerto La Cruz. Anzoátegui

          </div>
          <div class="text--bold text-white row text--new">
             <img src="Phone.svg" style="width:24px" alt="" srcset=""> <span class="q-pl-sm" >Teléfonos:</span>

          </div>
          <div class="text-white row text--new">
              0281-2688176  0281-3320023

          </div>
           <div class="text--bold text-white row text--new">
             <img src="Envelope.svg" style="width:24px" alt="" srcset=""> <span class="q-pl-sm" >Correo:</span>

          </div>
          <div class="text-white row text--new">
              ueisanlazaro@hotmail.com

          </div>

        </div>

        <div :class="$q.platform.is.mobile ? '' : 'justify-end q-pr-md'" class="col-md-8 text-center col-xs-6 col-sm-6 row ">

            <div class="text--bold text-white  text--new">
              <div>
                Siguenos en:
              </div>
              <div class="row q-gutters-md">
              <div class="col-4">
                <q-btn type="a" target="_blank" href="https://www.facebook.com/UEI-San-L%C3%A1zaro-II-154461703034193/"  flat>
                   <img src="/Facebook.svg" alt="" :style="$q.platform.is.mobile ?'width:40px' :'width:50px'" srcset="">
                </q-btn>
               
              </div>
              <div class="col-4">
                <q-btn type="a" target="_blank" href="https://instagram.com/uei_san_lazaro_ii_plc?igshid=YmMyMTA2M2Y=" flat>
                   <img src="/Instagram.svg" :style="$q.platform.is.mobile ?'width:40px' :'width:50px'" rcset="">
                </q-btn>
                

              </div>
              <div class="col-4">
                <q-btn type="a" target="_blank" flat href="https://wa.me/+584248880834?text=¡Hola!" >
                  <img src="/WhatsApp.svg" :style="$q.platform.is.mobile ?'width:40px' :'width:50px'"  srcset="">
                </q-btn>
                  
              </div>
            </div>
            </div>

        </div>
      </div>
  </div>
</template>

<script>
export default {
   name: 'footer-v',
  setup () {
    return {}
  }
}
</script>
