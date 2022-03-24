<template>
  <div class="featuredZone">
    <a class="featuredBox" id="featured1" :href="link1">
      <div class="featuredText">
        <h1>{{ featuredTextOne }}</h1>
      </div>
    </a>
    <a class="featuredBox" id="featured2" :href="link2">
      <div class="featuredText">
        <h1>{{ featuredTextTwo }}</h1>
      </div>
    </a>
    <a class="featuredBox" id="featured3" :href="link3">
      <div class="featuredText">
        <h1>{{ featuredTextThree }}</h1>
      </div>
    </a>
    <a class="featuredBox" id="featured4" :href="link4">
      <div class="featuredText">
        <h1>{{ featuredTextFour }}</h1>
      </div>
    </a>
  </div>
</template>

<script>
export default {
  name: 'FeaturedZone',
  props: {
    featuredTextOne: String,
    featuredTextTwo: String,
    featuredTextThree: String,
    featuredTextFour: String,
    link1: String,
    link2: String,
    link3: String,
    link4: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
a {
  text-decoration: none;
}
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
  background-image: url("@/assets/que-ver.jpg");
  background-size: cover;
}
#featured2 {
  background-image: url("@/assets/gastronomia.jpg");
  background-size: cover;
}
#featured3 {
  background-image: url("@/assets/naturaleza.jpg");
  background-size: cover;
}
#featured4 {
  background-image: url("@/assets/historia.jpg");
  background-size: cover;
}
.featuredText {
  display: block;
  background-color: black;
  color: white;
}
</style>
