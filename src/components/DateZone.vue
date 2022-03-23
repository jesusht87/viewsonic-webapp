<template>
  <div class="dateZone">
    <div class="dateInfo">
      {{getDate()}}  |  {{getHour()}}
    </div>
    <div class="elfsight-app-6d87e46d-f9aa-48fa-a49f-6f7c673da185 weatherInfo">
    </div>
  </div>
</template>

<script>
export default {
  name: 'DateZone',
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
  justify-content: space-between;
  align-items: center;
  height: auto;
  padding-top: 50px;
  padding-bottom: 15px;
  background-image: url("@/assets/dateZoneBg.jpg");
  background-size: cover;
}
.dateInfo {
  display: block;
  margin-left: 20%;
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
