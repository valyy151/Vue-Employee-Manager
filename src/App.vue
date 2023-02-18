<template>
	<Navbar />
	<Employees :employees="employees" />
</template>

<script>
	import Navbar from './components/Vue-Navbar.vue';
	import Employees from './components/Vue-Employees.vue';
	export default {
		name: 'App',
		components: { Navbar, Employees },
		data() {
			return { employees: [] };
		},
		created() {
			this.employees = [
				{
					verified: false,
					id: 1,
					name: 'Jack Jackson',
					begin: 14,
					end: 22,
					hours: 8,
					date: Date.now,
				},
				{
					verified: false,
					id: 2,
					name: 'Susan Garcia',
					begin: 14,
					end: 22,
					hours: 8,
					date: Date.now,
				},
				{
					verified: false,
					id: 3,
					name: 'David Samuels',
					begin: 16,
					end: 23,
					hours: 7,
					date: Date.now,
				},
				{
					verified: true,
					id: 4,
					name: 'Ruth Huggins',
					begin: 16,
					end: 23,
					hours: 7,
					date: Date.now,
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
