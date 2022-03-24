<template>
  <div class="home">
    <HeroZone :heroMessage="'Welcome!'" />
    <DateZone :hashtagMessage="'#IngenioInvitesToFeel'" />
    <FeaturedZone :featuredTextOne="'What to see'" :featuredTextTwo="'Gastronomy'" :featuredTextThree="'Nature'" :featuredTextFour="'History'"
    :link1="'https://turismoingenio.com/que-ver/?lang=en'"
    :link2="'https://turismoingenio.com/gastronomia-ingenio/?lang=en'"
    :link3="'https://turismoingenio.com/natur/?lang=en'"
    :link4="'https://turismoingenio.com/patrimonio/?lang=en'"/>
    <CallToActionZone :message="'Have you had your breakfast?'" :message2="'Discover the authentic flavors of Ingenio today... Are you up to?'"/>
  </div>
</template>

<script>
// @ is an alias to /src
import HeroZone from '@/components/HeroZone.vue'
import DateZone from '@/components/DateZone.vue'
import FeaturedZone from '@/components/FeaturedZone.vue'
import CallToActionZone from '@/components/CallToActionZone.vue'

export default {
  name: 'EnglishView',
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
