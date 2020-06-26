<template lang="pug">
  #login.wrap
    img(alt="Vue logo" src="@/assets/images/satellite-platzi.png")
    h1.title Registro estación de Platzi
    label Nombre
    input.input(type='text')
    label Apellido
    input.input(type='text')
    label Cargo
    input.input(type='text')
    button.button.is-primary Enviar
</template>

<script>
export default {
  name: "HelloWorld",
  props: {
    msg: String
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss" scoped>
@import "@/assets/scss/main.scss";

.wrap {
  width: 320px;
  height: 409px;
  display: grid;
  margin: auto;
}

h1.title {
  font-weight: bold;
}

#login img {
  margin: 0 auto 20px;
}

#login label {
  text-align: left;
  margin: 20px 0 10px;
  color: #ff9300;
  font-weight: 600;
  font-size: 0.8em;
}

#login input {
  width: auto;
  height: 50%;
  border: 0;
  border-bottom: 1px solid #ff9300;
  border-radius: 0;
}

#login button {
  margin-left: auto;
  width: 25%;
  height: 50%;
  margin-top: 20px;
}

// h3 {
//   margin: 40px 0 0;
// }
// ul {
//   list-style-type: none;
//   padding: 0;
// }
// li {
//   display: inline-block;
//   margin: 0 10px;
// }
// a {
//   color: #42b983;
// }
</style>
