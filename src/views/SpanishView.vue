<template>
  <div class="home">
    <HeroZone :heroMessage="'¡Bienvenid@s!'" />
    <DateZone />
    <FeaturedZone />
    <DiscoverZone />
  </div>
</template>

<script>
// @ is an alias to /src
import HeroZone from '@/components/HeroZone.vue'
import DateZone from '@/components/DateZone.vue'
import FeaturedZone from '@/components/FeaturedZone.vue'
import DiscoverZone from '@/components/DiscoverZone.vue'

export default {
  name: 'SpanishView',
  components: {
    HeroZone,
    DateZone,
    FeaturedZone,
    DiscoverZone
  }
}
</script>

<style lang="scss">
.home {
  width: 100%;
}
</style>
