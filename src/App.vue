<template>
<h1>Ejemplo</h1>
<h2>Por favor, digite su nombre</h2>
<input type="text" v-model="name" />
<button v-on:click="sayHello()">Saludar</button>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data(){
	return {
		name:''
	}
  },
  methods:{
	sayHello(){
		alert("hola "+this.name)

	}
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
