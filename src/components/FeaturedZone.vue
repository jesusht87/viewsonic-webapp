<template>
  <div class="featuredZone">
    <div class="featuredBox" id="featured1">
      <div class="featuredText">
        <h1> {{featuredTextOne}} </h1>
      </div>
    </div>
    <div class="featuredBox" id="featured2">
      <div class="featuredText">
      <h1> {{featuredTextTwo}} </h1>
      </div>
    </div>
    <div class="featuredBox" id="featured3">
      <div class="featuredText">
        <h1> {{featuredTextThree}} </h1>
      </div>
    </div>
    <div class="featuredBox" id="featured4">
      <div class="featuredText">
        <h1> {{featuredTextFour}} </h1>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DateZone',
  data () {
    return {
      featuredTextOne: 'Qué ver',
      featuredTextTwo: 'Gastronomía',
      featuredTextThree: 'Naturaleza',
      featuredTextFour: 'Historia'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.featuredZone {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: auto;
  padding-top: 50px;
  padding-bottom: 15px;
  background-color: white;
}
.featuredBox {
  display: block;
  margin: 1%;
  width: 100%;
  height: 480px;
  box-shadow: 0px 0px 15px 0px, 0px 0px 0px 0px rgba(182, 182, 182, 0);
}
#featured1 {
  background-image: url('@/assets/que-ver.jpg');
  background-size: cover;
}
#featured2 {
  background-image: url('@/assets/gastronomia.jpg');
  background-size: cover;
}
#featured3 {
  background-image: url('@/assets/naturaleza.jpg');
  background-size: cover;
}
#featured4 {
  background-image: url('@/assets/historia.jpg');
  background-size: cover;
}
.featuredText {
  display: block;
  background-color: black;
  color: white;
}
</style>
