<template>
	<header>
		<div class="logo"><a href="">App</a></div>
		<div class="links">
			<a href="">Home</a>
			<a href="">About</a>
			<a href="">Support</a>
			<a href="">Login</a>
		</div>
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
