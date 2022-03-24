<template>
  <div class="heroMain">
    <div class="heroMessage">
    <h1>{{heroMessage}}</h1>
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeroZone',
  props: {
    heroMessage: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
.heroMain {
  display: flex;
  justify-content: center;
  align-items: center;
  background-image: url("@/assets/heroBackground.jpg");
  background-size: cover;
  height: 450px;
}
.heroMessage {
  display: block;
  font-family: 'Norican', sans-serif;
  font-size: xx-large;
  color: white;
}
</style>
