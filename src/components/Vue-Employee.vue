<template>{{ employee.name }}</template>

<script>
	export default {
		name: 'Vue-Employee',
		props: {
			verified: Boolean,
			id: Number,
			name: String,
			begin: Number,
			end: Number,
			hours: Number,
			date: Date,
		},
	};
</script>
