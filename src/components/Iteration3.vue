<script setup>
	import { ref } from "vue";

	const hello = ref(true);
</script>

<template>
	<h3>iteration 3</h3>
	<p v-if="hello">Hello my Name is Judit</p>
</template>


<style scoped>
	h3 {
		margin-top: 20px;
	}
</style>