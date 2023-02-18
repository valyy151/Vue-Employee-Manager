<template>
	<header>
		<div class="logo"><router-link to="/">App</router-link></div>
		<div class="links">
			<router-link to="/">Home</router-link>
			<router-link to="/about">About</router-link>
			<router-link to="/support">Support</router-link>
			<router-link to="/login">Login</router-link>
		</div>
		<router-view />
	</header>
</template>

<script>
	export default {
		name: 'Vue-Navbar',
	};
</script>

<style scoped>
	header {
		display: flex;
		background-color: #3eaf7c;
		padding: 10px 0;
	}
	header a {
		color: white;
		text-decoration: none;
		font-size: 1.2em;
	}
	.logo {
		margin: 0 auto 0 35px;
	}

	.links {
		display: flex;
		justify-content: space-evenly;
		width: 20%;
	}
</style>
