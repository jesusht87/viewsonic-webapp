<template>
  <div class="home">
    <HeroZone :heroMessage="'Willkommen!'" />
    <DateZone :hashtagMessage="'#IngenioLädtZumFühlenEin'" />
    <FeaturedZone :featuredTextOne="'Was zu Sehen'" :featuredTextTwo="'Gastronomie'" :featuredTextThree="'Natur'" :featuredTextFour="'Geschichte'"
    :link1="'https://turismoingenio.com/que-ver/?lang=de'"
    :link2="'https://turismoingenio.com/gastronomia-ingenio/?lang=de'"
    :link3="'https://turismoingenio.com/natur/?lang=de'"
    :link4="'https://turismoingenio.com/patrimonio/?lang=de'"/>
    <CallToActionZone :message="'Hattest du Frühstück?'" :message2="'Entdecken Sie noch heute die authentischen Aromen von Ingenio. Nicht verpassen!'"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeroZone from '@/components/HeroZone.vue'
import DateZone from '@/components/DateZone.vue'
import FeaturedZone from '@/components/FeaturedZone.vue'
import CallToActionZone from '@/components/CallToActionZone.vue'

export default {
  name: 'DeutschView',
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
