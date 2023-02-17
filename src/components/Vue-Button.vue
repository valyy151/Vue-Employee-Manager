<template>
	<div class="button">
		<button :style="{ background: color }">{{ text }}</button>
	</div>
</template>

<script>
	export default {
		name: 'Vue-Button',
		props: {
			text: String,
			color: String,
		},
	};
</script>

<style scoped>
	.button {
		margin-top: 100px;
	}
	.button button {
		padding: 5px 15px;

		border: 1px solid #3eaf7c;
		color: #3eaf7c;
		font-size: 1.2em;
		border-radius: 10px;
		cursor: pointer;
	}
</style>
