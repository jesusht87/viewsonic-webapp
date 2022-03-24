<template>
  <div class="home">
    <HeroZone :heroMessage="'¡Bienvenid@s!'" />
    <DateZone :hashtagMessage="'#IngenioTeInvitaASentir'" />
    <FeaturedZone :featuredTextOne="'Qué ver'" :featuredTextTwo="'Gastronomía'" :featuredTextThree="'Naturaleza'" :featuredTextFour="'Historia'"
    :link1="'https://turismoingenio.com/que-ver/'"
    :link2="'https://turismoingenio.com/gastronomia-ingenio/'"
    :link3="'https://turismoingenio.com/natur/'"
    :link4="'https://turismoingenio.com/patrimonio/'"/>
    <CallToActionZone :message="'¿Has desayunado?'" :message2="'Descubre los sabores más auténticos de Ingenio escaneando el código QR con tu móvil. ¿Te animas?'"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeroZone from '@/components/HeroZone.vue'
import DateZone from '@/components/DateZone.vue'
import FeaturedZone from '@/components/FeaturedZone.vue'
import CallToActionZone from '@/components/CallToActionZone.vue'

export default {
  name: 'SpanishView',
  components: {
    HeroZone,
    DateZone,
    FeaturedZone,
    CallToActionZone
  }
}
</script>

<style lang="scss">
.home {
  width: 100%;
}
</style>
