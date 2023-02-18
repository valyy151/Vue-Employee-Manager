<template>
	<li>{{ person.name }}</li>
	<li>Begin: {{ person.begin }}</li>
	<li>End: {{ person.end }}</li>
</template>

<script>
	export default {
		name: 'Vue-Person',
		props: {
			person: Object,
		},
	};
</script>
