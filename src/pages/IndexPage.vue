<template>
  <q-page>
    <div class="row">
        <div class="col-md-4 col-sm-12  banner q-pa-md">
          <div class="q-mt-xl q-pt-md title-v ">
            Un Mejor futuro
            para tus hijos
          </div>
          <div class="subtitle-v q-pt-sm">
        “La educación es el arma más
          poderosa que puedes usar para
          cambiar el mundo”
          </div>
          <div class="text-right subtitle-v q-pt-sm">
               Nelson Mandela.
          </div>

        </div>
        <div class="col-8" v-if="!$q.platform.is.mobile">

          <img src="/back.svg" style="width: 100%; " alt="" srcset="">
        </div>
        <div class="col-12 row">
          <div class="col-md-4 col-xs-12 col-sm-12">
            <InfoCardVue
            title="Visión"
            icon="/visionIcon.svg"
            background="/vision.jpg"
            btnClass="btn--blue1"
            cardClass="card--modal--vision"
            :left="false"
            >

        <p>
            Aquello a lo queremos avanzar a medio y largo plazo, es nuestra aspiración, nuestro deseo.

        </p>
        <p>
          Profundizar en nuestro trabajo para que seamos:
        </p>
        <p>
          Una institución, multidisciplinaria e integrada a su región y al mundo; destinada a impartir educación en los sub-sistemas de Educación Inicial, Educación Primaria y Educación Media General.
        </p>
        <p>
          Autónoma y concebida como un ámbito institucional con independencia académica, científica y económica. Libre de cualquier poder e influencia ideológica, política o religiosa.
        </p>
        <p>
De tradición humanista, científica y cultural cuya comunidad participe de la constante preocupación por alcanzar el saber universal y la verdad.

        </p>
        <p>
Que sostenga los principios democráticos de igualdad y libertad, el respeto por los derechos humanos, la ética y la justicia, las prácticas de tolerancia y el respeto por la diversidad cultural y que rechace toda forma de discriminación tal como lo demanda la Constitución de la República Bolivariana de Venezuela. Donde las ideas sean desarrolladas y discutidas libremente en un ambiente motivador para el estudio, la creación y el logro.

        </p>
        <p>
Una institución inmersa en el cambio constante y en la búsqueda de conocimiento que caracterizan al mundo contemporáneo, capaz de anticiparse a ellas y de convertirse en un agente positivo de estas transformaciones. Con vocación interdisciplinaria, que no limita su campo de acción y reflexión en el que combine diversas disciplinas que abarcan la cultura en un sentido amplio y que está integrado por las humanidades, las artes, las ciencias sociales, las ciencias básicas y la tecnología.

        </p>







            </InfoCardVue>
          </div>
          <div class="col-md-4 col-xs-12 col-sm-12">
            <InfoCardVue
            title="Misión"
            icon="/misionIcon.svg"
            background="/mision.jpg"
            btnClass="btn--green1"
            cardClass="card--modal--mision"
            :left="false"
            >
             <p>
          Aquello a cuyo cumplimiento debe dirigirse nuestro trabajo en el colegio, la razón de ser, aquello para lo que existimos:
         </p>

     <p>
      La Unidad Educativa Industrial San Lázaro II se caracteriza por ser una institución que busca el conocimiento como fin en sí mismo y también para ser aplicado en beneficio de la sociedad y de aquellos que lo poseen.
     </p>
     <p>
      Una institución cuyo fin primordial es impartir Educación Primaria y Educación Media General, centrando las miras en el sujeto que aprende con el propósito de fortalecer al máximo sus capacidades.
     </p>
     <p>
        Aquella que brindará servicios a su comunidad a través del desarrollo endógeno, buscando satisfacer sus necesidades.
     </p>
     <p>
      Que contribuye a expandir el conocimiento, a fomentar el desarrollo tecnológico, a estimular el surgimiento y la difusión de las ideas y promover la investigación e incentivar la creación.
     </p>
     <p>
      Capaz de generar innovación en los procesos de enseñanza, de manera tal que ayuden a identificar y resolver las cuestiones  que preocupan y afectan a la comunidad, contribuyendo al logro de la  paz, el desarrollo sostenible y mejoramiento de la condición humana.
     </p>
     <p>
      Nuestra principal misión es brindar una educación de calidad, centrando las miras en el sujeto que aprende con el propósito de fortalecer al máximo sus capacidades.
     </p>
     <p>
        En el plano social, contribuir a la expansión del conocimiento, la difusión de las ideas, la integración de la cultura.
     </p>
            </InfoCardVue>
          </div>
          <div class="col-md-4 col-xs-12 col-sm-12 ">
            <InfoCardVue
            title="¿Quienes somos?"
            icon="/quienes.svg"
            background="/quienes.jpg"
            btnClass="btn--blue1"
            cardClass="card--modal--vision"
            :left="true"

            >
           <p>
             Aquello a lo queremos avanzar a medio y largo plazo, es nuestra aspiración, nuestro deseo.

           </p>
           <p>
          Profundizar en nuestro trabajo para que seamos:

           </p>
           <p>
              Una institución, multidisciplinaria e integrada a su región y al mundo; destinada a impartir educación en los sub-sistemas de Educación Inicial, Educación Primaria y Educación Media General.

           </p>
           <p>
              Autónoma y concebida como un ámbito institucional con independencia académica, científica y económica. Libre de cualquier poder e influencia ideológica, política o religiosa.

           </p>
           <p>
              De tradición humanista, científica y cultural cuya comunidad participe de la constante preocupación por alcanzar el saber universal y la verdad.

           </p>
           <p>
Que sostenga los principios democráticos de igualdad y libertad, el respeto por los derechos humanos, la ética y la justicia, las prácticas de tolerancia y el respeto por la diversidad cultural y que rechace toda forma de discriminación tal como lo demanda la Constitución de la República Bolivariana de Venezuela. Donde las ideas sean desarrolladas y discutidas libremente en un ambiente motivador para el estudio, la creación y el logro.

           </p>
           <p>
Una institución inmersa en el cambio constante y en la búsqueda de conocimiento que caracterizan al mundo contemporáneo, capaz de anticiparse a ellas y de convertirse en un agente positivo de estas transformaciones. Con vocación interdisciplinaria, que no limita su campo de acción y reflexión en el que combine diversas disciplinas que abarcan la cultura en un sentido amplio y que está integrado por las humanidades, las artes, las ciencias sociales, las ciencias básicas y la tecnología.

           </p>













            </InfoCardVue>
          </div>
          <div class="col-12">
            <HistoryCardVue>

            </HistoryCardVue>
          </div>
          <div class="col-12">
              <SliderVue></SliderVue>
          </div>

        </div>
        <footer_v></footer_v>
    </div>

  </q-page>
</template>


<script>
import { defineComponent } from 'vue'
import InfoCardVue from 'components/commons/InfoCard.vue'
import HistoryCardVue from 'components/commons/HistoryCard.vue'
import SliderVue from 'components/commons/Slider.vue'
import footer_v from 'components/commons/Footer.vue'
import { useQuasar } from 'quasar'
export default defineComponent({
  name: 'IndexPage',
  components:{InfoCardVue, HistoryCardVue, SliderVue, footer_v},
  setup () {
    const $q = useQuasar();
    return{ $q}
  }
})
</script>
