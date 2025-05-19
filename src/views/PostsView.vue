<template>
	<div class="posts container">
		<!-- <img alt="mazebook" src="../assets/img/wordmark.svg" class="logo" /> -->
		<CardComp
			class="mt-4 mx-auto single-spot"
			picture="https://blobdojo.blob.core.windows.net/micontenedor/804443cb-ac59-408a-a1f6-5d33cbf4ea2c.jpg"
			parrafo="Hermosa Ciudad"
			:header="{
				name: 'Diego Bueno',
				picture: 'https://blobdojo.blob.core.windows.net/micontenedor/73ec9041-c515-4886-ab7b-9411565ac4a2.jpg',
			}"
			:likes="true" />
		<CardComp
			class="mt-4 mx-auto single-spot"
			picture="https://blobdojo.blob.core.windows.net/micontenedor/10772f6d-04b8-483e-8efa-06d2d594b05b.jpg"
			parrafo="Gran hazaña de Aliaaaaaaaaanza!!!"
			:header="{
				name: 'Diego Bueno',
				picture: 'https://blobdojo.blob.core.windows.net/micontenedor/73ec9041-c515-4886-ab7b-9411565ac4a2.jpg',
			}"
			:likes="true" />
		<CardComp
			class="mt-4 mx-auto single-spot"
			picture="https://blobdojo.blob.core.windows.net/micontenedor/5a7cec01-207c-4655-a48b-03ff11234573.jpg"
			parrafo="Tarapoto es lo máximo"
			:header="{
				name: 'Diego Bueno',
				picture: 'https://blobdojo.blob.core.windows.net/micontenedor/73ec9041-c515-4886-ab7b-9411565ac4a2.jpg',
			}"
			:likes="true" />
	</div>
</template>
<script>
	import CardComp from '../components/CardComp.vue'
	export default {
		name: 'PostsView',
		components: {
			CardComp,
		},
	}
</script>
<style scoped>
	.posts {
		min-height: 60vh;
		max-width: 895px;
		margin: auto;
	}
	.single-spot {
		max-width: 550px;
	}
	.logo {
		max-width: 115px;
		padding: 0.2rem;
	}
</style>
