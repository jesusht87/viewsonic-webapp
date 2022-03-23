<template>
  <div class="home">
    <HeroZone :heroMessage="'¡Bienvenid@s!'" />
    <DateZone />
    <FeaturedZone />
    <DiscoverZone />
    <CallToActionZone :message="'¿Has desayunado?'" :message2="'Descubre los sabores más auténticos de Ingenio escaneando el código QR con tu móvil. ¿Te animas?'"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeroZone from '@/components/HeroZone.vue'
import DateZone from '@/components/DateZone.vue'
import FeaturedZone from '@/components/FeaturedZone.vue'
import DiscoverZone from '@/components/DiscoverZone.vue'
import CallToActionZone from '@/components/CallToActionZone.vue'

export default {
  name: 'SpanishView',
  components: {
    HeroZone,
    DateZone,
    FeaturedZone,
    DiscoverZone,
    CallToActionZone
  }
}
</script>

<style lang="scss">
.home {
  width: 100%;
}
</style>
