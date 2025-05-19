<!-- <template>
	<div class="home">
		<div class="row mx-0">
			<div class="col-lg-12">
				<card-comp :btns="btnArray" class="mx-auto card-comp">
					<template #default>
						<form>
							<div class="mb-3 mt-2">
								<input
									type="email"
									class="form-control"
									placeholder="Ingresa tu email" />
							</div>
							<div class="mb-3 mt-2">
								<input
									type="password"
									class="form-control"
									placeholder="Contraseña" />
							</div>
						</form>
					</template>
					<template v-slot:footer>
						<hr />
						<button class="btn btn-success">Crear cuenta</button>
					</template>
				</card-comp>
			</div>
		</div>
	</div>
</template>

<script>
	// @ is an alias to /src
	import CardComp from '../components/CardComp.vue'

	export default {
		name: 'HomeView',
		components: {
			CardComp,
		},

		data() {
			return {
				btnArray: [
					{
						txt: 'Iniciar sesión',
						class: 'btn-primary',
					},
					{
						txt: 'Has olvidado tu contraseña?',
						class: '',
					},
				],
			}
		},
	}
</script>

<style scoped>
	h2 {
		max-width: 470px;
		margin: auto;
		font-size: 1.8rem;
	}
	.home {
		max-width: 895px;
		margin: auto;
	}
	.img-cont {
		display: flex;
		flex-direction: column;
	}

	img {
		max-width: 315px;
		margin: 1em auto 0 auto;
	}

	.card-comp {
		max-width: 398px;
	}
	.btn-success {
		margin: auto;
		min-width: 195px;
	}

	@media (min-width: 992px) {
		.home {
			margin: 4em auto;
		}
		img {
			margin: 0;
			margin-top: 5.6em;
		}
		h2 {
			margin: 0;
			margin-top: -0.8em;
			margin-left: 0.8em;
		}
		.card-comp {
			margin-top: 3rem;
		}
	}
</style> -->

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
