<script setup>
	import { ref } from "vue";

	const string = () => {
		return "Hello World";
	};
</script>

<template>
	<div>
		<h3>iteration 1</h3>
		<p>{{ string() }}</p>
	</div>
</template>


<style lang="scss" scoped>
</style>