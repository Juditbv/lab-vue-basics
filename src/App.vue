<script setup>
	import HeaderGeneral from "./components/HeaderGeneral.vue";
	import FooterGeneral from "./components/FooterGeneral.vue";
	import Iteration2 from "./components/Iteration2.vue";
	import Iteration3 from "./components/Iteration3.vue";
</script>

<template>
	<HeaderGeneral />
	<main>
		<Iteration2 />
		<Iteration3 />
	</main>
	<FooterGeneral />
</template>

<style scoped>
	main {
		margin: 100px 0;
	}
</style>
