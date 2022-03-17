<template>
	<b-container class="pt-5 my-5" id="tecnologias">
		<div class="text-center my-5">
			<h2 class="font-bold size20">TECNOLOGÍAS</h2>
			<p>Estas son algunas de las tecnologías que he aprendido</p>
		</div>

		<div class="slider">
			<div class="slide-track">
				<div v-for="(item, index) in logos" :key="index" class="slide">
					<img :src="item.route" height="100" width="100" /> <br />
					<p v-text="item.nombre" class="mt-2 fw-bold"></p>
				</div>
			</div>
		</div>
	</b-container>
</template>

<script>
	export default {
		name: "Tools",
		data() {
			return {
				logos: [
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/bootstrap.png",
						nombre: "BOOTSTRAP",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/css.png",
						nombre: "CSS",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/cypress.webp",
						nombre: "CYPRESS",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/firebase.webp",
						nombre: "FIREBASE",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/git.png",
						nombre: "GIT",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/html.png",
						nombre: "HTML",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/js.png",
						nombre: "JAVASCRIPT",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/npm.png",
						nombre: "NPM",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/sass.png",
						nombre: "SAAS",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/vue.png",
						nombre: "VUE",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/bootstrap.png",
						nombre: "BOOTSTRAP",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/css.png",
						nombre: "CSS",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/cypress.webp",
						nombre: "CYPRESS",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/firebase.webp",
						nombre: "FIREBASE",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/git.png",
						nombre: "GIT",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/html.png",
						nombre: "HTML",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/js.png",
						nombre: "JAVASCRIPT",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/npm.png",
						nombre: "NPM",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/sass.png",
						nombre: "SAAS",
					},
					{
						route: "https://raw.githubusercontent.com/leoaceituno/Files/main/vue.png",
						nombre: "VUE",
					},
				],
			};
		},
	};
</script>

<style scoped>
	body {
		align-items: center;
		justify-content: center;
	}
	@keyframes scroll {
		0% {
			transform: translateX(0);
		}
		100% {
			transform: translateX(calc(-250px * 10));
		}
	}

	.slider {
		height: 150px;
		margin: auto;
		overflow: hidden;
		position: relative;
		width: auto;
		text-align: center;
	}
	.slide-track {
		animation: scroll 40s linear infinite;
		display: flex;
		width: calc(250px * 20);
	}
	.slide {
		height: 100px;
		width: 250px;
	}
</style>