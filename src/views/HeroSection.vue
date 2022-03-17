<template>
	<b-container class="pt-5 my-5">
		<div
			class="d-flex justify-content-between align-items-center my-5 py-5"
		>
			<div>
				<h1 class="size46 font-black">LEONARDO ACEITUNO</h1>
				<p class="size20">FRONT-END WEB DEVELOPER</p>
				<p>Vue.js | JavaScript | HTML | CSS</p>

				<b-link
					v-for="(item, index) in iconos"
					:key="index"
					:href="item.to"
					target="_blank"
					class="me-4 link"
				>
					<b-icon :icon="item.nombre" font-scale="2"></b-icon>
				</b-link>
			</div>
			<div>
				<b-img
					src="https://media0.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif"
					width="400"
				></b-img>
			</div>
		</div>
		<!-- 
			src="https://cdn.dribbble.com/users/320114/screenshots/2575134/code_dribbble.gif"
			src="https://media0.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif"
		/> -->
	</b-container>
</template>

<script>
	export default {
		name: "HeroSection",
		data() {
			return {
				iconos: [
					{ nombre: "github", to: "https://www.github.com" },
					{ nombre: "twitter", to: "https://twitter.com/home" },
					{ nombre: "linkedin", to: "https://www.linkedin.com/feed/" },
				],
				color: "#003140",
			};
		},
	};
</script>

<style scoped>
	.link {
		color: #00b1de !important;
	}
</style>