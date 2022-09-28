<script setup>
	import { ref } from "vue";
	const allPosts = ref([
		{
			title: "Hello 1",
			description: "hola hola qui soc",
			content:
				"Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laboriosam quas incidunt quaerat accusantium saepe dolores nulla autem repellat facere earum ab dignissimos asperiores iure rerum consequuntur, soluta, iusto quos odit?",
		},
		{
			title: "Hello 2",
			description: "holi holi soc la Judit",
			content:
				"Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laboriosam quas incidunt quaerat accusantium saepe dolores nulla autem repellat facere earum ab dignissimos asperiores iure rerum consequuntur, soluta, iusto quos odit?",
		},
		{
			title: "Hello 3",
			description: "cada dia al dematí",
			content:
				"Lorem ipsum dolor sit amet, consectetur adipisicing elit. Laboriosam quas incidunt quaerat accusantium saepe dolores nulla autem repellat facere earum ab dignissimos asperiores iure rerum consequuntur, soluta, iusto quos odit?",
		},
	]);

	let changeBg = ref("bg-1");
</script>

<template>
	<h3>iteration 4</h3>
	<div class="flex">
		<div v-for="post in allPosts" :key="post" class="card" :class="changeBg">
			<h2>{{ post.title }}</h2>
			<h4>{{ post.description }}</h4>
			<p>{{ post.content }}</p>
		</div>
	</div>

	<h3>iteration 5</h3>
	<button @click="changeBg = 'bg-2'">change color cards</button>
</template>


<style scoped>
	h3 {
		margin-top: 20px;
	}

	.flex {
		display: flex;
		align-items: center;
		justify-content: space-evenly;
	}

	.card {
		padding: 20px;
		color: black;
		margin: 30px;
	}

	.bg-1 {
		background-color: darkseagreen;
	}

	.bg-2 {
		background-color: bisque;
	}

	.card h2 {
		font-weight: 600;
		margin-bottom: 10px;
	}

	.card h4 {
		font-style: oblique;
	}

	p {
		margin-top: 20px;
	}
</style>