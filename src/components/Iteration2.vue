<script setup>
	import { ref } from "vue";

	const string = () => {
		return "Hello World";
	};
</script>

<template>
	<div>
		<h3>iteration 2</h3>
		<p>{{ 2 + 2 }}</p>
		<p>{{ string() }}</p>
	</div>
</template>


<style scoped>
</style>