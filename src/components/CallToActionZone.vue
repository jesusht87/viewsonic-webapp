<template>
  <div class="callToActionMain">
    <div class="callToActionMessageZone">
      <h2>{{message}}</h2>
      <h4>{{message2}}</h4>
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
  margin-top: 10px;
  height: 800px;
  background-image: url("@/assets/desayunos.jpg");
  background-size: contain;
  background-repeat: no-repeat;
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
