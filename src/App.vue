<template>
	<Navbar />

	<Button
		color="none"
		text="Add Task" />
</template>

<script>
	import Navbar from './components/Vue-Navbar.vue';
	import Button from './components/Vue-Button.vue';

	export default {
		name: 'App',
		components: { Navbar, Button },
	};
</script>

<style>
	#app {
		font-family: Avenir, Helvetica, Arial, sans-serif;
		-webkit-font-smoothing: antialiased;
		-moz-osx-font-smoothing: grayscale;
		text-align: center;
		color: #2c3e50;
	}
</style>
