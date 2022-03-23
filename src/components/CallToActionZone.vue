<template>
  <div class="callToActionMain">
    <div class="callToActionMessageZone">
      <h1>{{message}}</h1>
      <h2>{{message2}}</h2>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CallToActionZone',
  props: {
    message: String,
    message2: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.callToActionMain {
  display: flex;
  justify-content: center;
  margin-top: 100px;
  height: 960px;
  background-image: url("@/assets/desayunos.jpg");
  background-size: cover;
}
.callToActionMessageZone {
  display: block;
  margin-left: 10%;
  margin-right: 40%;
  font-family: 'Fredoka', sans-serif;
  text-align: left;
  font-size: xx-large;
  color: black;
}
</style>
