<template>
  <div class="heroMain">
    <div>
    <img class="logo" src="@/assets/logo.png">
    </div>
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
  padding-top: 15%;
  height: 480px;
  background-image: url("@/assets/heroBackground.jpg");
  background-size: cover;
}
.heroMessage {
  display: block;
  margin-left: 10%;
  font-family: 'Norican', sans-serif;
  font-size: xx-large;
  color: white;
}
.logo {
  display: block;
  max-width: 350px;
  margin-right: 10%;
}
</style>
