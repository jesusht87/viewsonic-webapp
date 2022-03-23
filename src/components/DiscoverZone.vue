<template>
<div class="discoverZoneContainer">
  <div class="discoverZoneTitle">
    <h1>{{discoverZoneTitle}}</h1>
  </div>
  <div class="discoverZone">
    <div class="discoverBox" id="discover1">
      <div class="discoverText">
        <h1> {{discoverTextOne}} </h1>
      </div>
    </div>
    <div class="discoverBox" id="discover2">
      <div class="discoverText">
      <h1> {{discoverTextTwo}} </h1>
      </div>
    </div>
    <div class="discoverBox" id="discover3">
      <div class="discoverText">
        <h1> {{discoverTextThree}} </h1>
      </div>
    </div>
    <div class="discoverBox" id="discover4">
      <div class="discoverText">
        <h1> {{discoverTextFour}} </h1>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'DateZone',
  data () {
    return {
      discoverZoneTitle: 'Ingenio, te invita a sentir...',
      discoverTextOne: 'Guayadeque',
      discoverTextTwo: 'El Mar y las Olas',
      discoverTextThree: 'El Deporte',
      discoverTextFour: 'La Artesanía'
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

.discoverZone {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: auto;
  padding-top: 50px;
}
.discoverZoneContainer {
  background-image: url("@/assets/discoverBg.jpg");
  background-size: cover;
  padding-bottom: 100px;
  margin-top: 100px;
  margin-bottom: 100px;
}
.discoverZoneTitle {
  margin-bottom: -20px;
  padding-top: 20px;
  padding-bottom: 20px;
}
.discoverZoneTitle h1 {
  font-family: 'Norican', sans-serif;
  font-size: 80px;
}
.discoverBox {
  display: block;
  margin: 1%;
  width: 100%;
  height: 480px;
  box-shadow: 0px 0px 15px 0px, 0px 0px 0px 0px rgba(182, 182, 182, 0);
}
#discover1 {
  background-image: url('@/assets/que-ver.jpg');
  background-size: cover;
}
#discover2 {
  background-image: url('@/assets/gastronomia.jpg');
  background-size: cover;
}
#discover3 {
  background-image: url('@/assets/naturaleza.jpg');
  background-size: cover;
}
#discover4 {
  background-image: url('@/assets/historia.jpg');
  background-size: cover;
}
.discoverText {
  background-color: black;
  color: white;
}
</style>
