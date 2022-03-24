<template>
  <div class="dateZone">
    <div class="dateInfo">
      <h3> {{ hashtagMessage }} </h3>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DateZone',
  props: {
    hashtagMessage: String
  },
  methods: {
    getDate () {
      const date = new Date()
      return String(date.getDate()).padStart(2, '0') + '/' + String(date.getMonth() + 1).padStart(2, '0') + '/' + date.getFullYear()
    },
    getHour () {
      const now = new Date()
      return now.getHours() + ':' + now.getMinutes()
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.dateZone {
  display: flex;
  justify-content: center;
  height: auto;
  padding-top: 20px;
  padding-bottom: 15px;
  background-image: url("@/assets/dateZoneBg.jpg");
  background-size: cover;
}
.dateInfo {
  display: block;
  text-align: center;
  font-family: 'Fredoka', sans-serif;
  font-size: 50px;
  color: white;
}
.weatherInfo {
  display: block;
  margin-right: 20%;
  color: white;
}
</style>
