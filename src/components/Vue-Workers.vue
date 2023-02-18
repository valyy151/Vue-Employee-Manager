<template>
	<div>
		<ul
			:key="worker.id"
			v-for="worker in workers"
		>
			<Person :person="worker" />
		</ul>
	</div>
</template>

<script>
	import Person from './Vue-Person.vue';
	export default {
		name: 'Vue-Workers',
		components: {
			Person,
		},
		props: {
			workers: Array,
		},
	};
</script>

<style scoped>
	h3 {
		font-weight: 300;
	}
	ul,
	li {
		list-style: none;
		padding: 0;
		line-height: 2em;
		border: 1px solid seagreen;
	}
</style>
