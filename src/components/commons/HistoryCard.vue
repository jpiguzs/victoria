<template>
  <div>
    <q-card class=" full-width card--info--2 text-white">
      <div class="row">
        <div class="col-8">
          <div class="q-pl-xl">
           <img  src="~assets/logo.png" alt=""  style="width: 316.79px;
            height: 342px;" srcset=""/>

        </div>
        </div>
        <div class="col-4">
            <div class="text-white text-center title-v">
              Historia
            </div>
            <div>
              <div class=" q-pa-xl text-white text-center subtitle-v">
             ¡Más de 21 años educando!
            </div>
            <div class="flex flex-center">
              <q-btn class="btn--green1 btn--vic" label="Ver más" @click="showModal=!showModal"></q-btn>
            </div>
            </div>
        </div>
      </div>
        
    </q-card>
       <q-dialog v-model="showModal"
    
     transition-show="slide-up"
      transition-hide="slide-down"
    >
    <q-card class="card--modal--history">
      <div class="row">
        <div class=" col-10 q-pa-md row">
          <div class="col-6">
                 <img src="~assets/logo.png"  style="width: 75px;
                  height: 75px;" alt="" srcset="">
          </div>
          <div class="col-2 q-pt-md text-center text-white text--bold  text-h4">
                Historia
          </div>
       
        </div>
        
          <q-space />

          <q-btn icon="cancel" class="text-white btn--close" dense  flat v-close-popup></q-btn>
            
        </div>
        <q-card-section class="text-white text-justify text-data">
          <p>
         La Unidad Educativa Industrial “San Lázaro II” se encuentra ubicada en la Avenida Bolívar Sector Barrio Obrero en la Ciudad de Puerto La Cruz, Municipio Juan Antonio Sotillo, Estado Anzoátegui. En ésta populosa avenida se encuentra variedades de comercios dedicados a la venta de repuestos automovilísticos, así como también concesionarios. Se conecta al Paseo Miranda con la Avenida Intercomunal Jorge Rodríguez (antigua Avenida Andrés Bello), dicha avenida ayuda en gran medida a los transportes terrestres. 

          </p>
          <p>
            La Unidad Educativa Colegio San Lázaro fue fundada en el 01 de Septiembre de 2001. Ubicada en la Avenida Bolívar 262 Edificio Moderno en Puerto La Cruz en el Estado Anzoátegui lleva este nombre en agradecimiento de parte del Ing. Mauro Zelaya a su santo patrón San Lázaro.           

          </p>
          <p>
La institución tuvo como Director a el Profesor Jesús Rodríguez Marcano quien fue la cabeza de esta institución por dos años. En la plana directiva se encontraba la Profesora Zaida Rodríguez como coordinadora académica y la profesora Elsa Rodríguez de Rivas como jefa del Departamento de Control de Estudios. 

          </p>
          <p>
Desde hace siete años la Dirección del Plantel se encuentra a cargo del Profesor Francisco Rivas Risquez. La Institución funciona en horario Integral desde las 7:00 am hasta las 1:20 pm., atendiendo a  412 estudiantes, desde eI grupo de Educación Inicial hasta 5to año de Educación Media General, además algunos estudiantes reciben atención especial a través del especialista del área de dificultad del aprendizaje contratado por la institución. 

          </p>
          <p>
El área de Educación Física y Deporte está conformada por 1 especialista con un plan de trabajo para aumentar el rendimiento físico y mental de los estudiantes de los sub-sistemas de educación inicial, primaria y bachillerato. 

          </p>
          <p>
            
          </p>




        


      









        </q-card-section>
     
    </q-card>

    </q-dialog>
  </div>
</template>

<script>
import { ref } from 'vue'


export default {
  // name: 'ComponentName',
  setup () {
    return {
      showModal:ref(false)      
    }
  }
}
</script>
