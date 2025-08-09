<script>
export default {
	data(){
		return {
			name: 'Jace',
			status: 'running', // Status: Sleeping, Running, Idle
			tasks: ['Task 1', 'Task 2', 'Task 3' ],
			link: 'https://google.com'
		};
	},

	methods: {
		toggleStatus() {
			if (this.status === 'active'){
				this.status = 'pending';
			} else if (this.status === 'pending'){
				this.status = 'inactive';
			} else {
				this.status = 'active';
			}
		}
	}
};
</script>

<template>
	<h1>Hi {{ name }}! You did open this site!</h1>
	<p v-if="status === 'pending'"> Sleeping! </p>
	<p v-else-if="status === 'running'"> Running! </p>
	<p v-else="status === 'idle'"> Idle! </p>

	<h3> Tasks:</h3>
	<ul>
		<li v-for="task in tasks" key="task"> {{ task }} </li>
	</ul>
	<a :href="link"> Click for Google! </a>
	</br>
	<button @:click="toggleStatus"> Change Status </button>
</template>

<style></style>
