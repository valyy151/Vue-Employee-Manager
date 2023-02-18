<template>
	<div
		:key="employee.id"
		v-for="employee in employees"
	>
		{{ employee.name }}
	</div>
</template>

<script>
	import Employee from './Vue-Employee.vue';
	export default {
		name: 'Vue-Employees',
		props: {
			employees: Array,
		},
		components: Employee,
		data() {
			return {
				employee: {},
			};
		},
	};
</script>

<style scoped>
	ul {
		list-style: none;
	}
	h1 {
		font-weight: 300;
	}
</style>
