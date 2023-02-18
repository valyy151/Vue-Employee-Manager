<template>
	<Navbar />
	<Workers :workers="workersArray" />
</template>

<script>
	import { toNumber } from '@vue/shared';
	import Navbar from './components/Vue-Navbar.vue';
	import Workers from './components/Vue-Workers.vue';

	export default {
		name: 'App',
		components: { Navbar, Workers },
		data() {
			return { workersArray: [] };
		},
		created() {
			this.workersArray = [
				{
					id: 1,
					name: 'Jack Jackson',
					begin: toNumber('12:00'),
					end: toNumber('20:00'),
					date: toNumber('18.02.2023'),
				},
				{
					id: 2,
					name: 'Susan Garcia',
					begin: toNumber('12:00'),
					end: toNumber('20:00'),
					date: toNumber('18.02.2023'),
				},
				{
					id: 3,
					name: 'David Samuels',
					begin: toNumber('12:00'),
					end: toNumber('20:00'),
					date: toNumber('18.02.2023'),
				},
				{
					id: 4,
					name: 'Ruth Huggins',
					begin: toNumber('12:00'),
					end: toNumber('20:00'),
					date: toNumber('18.02.2023'),
				},
			];
		},
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

	nav {
		padding: 30px;
	}

	nav a {
		font-weight: bold;
		color: #2c3e50;
	}

	nav a.router-link-exact-active {
		color: #42b983;
	}
</style>
