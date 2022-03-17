<template>
	<div class="home">
		<HeroSection />
		<Tecnologias />
	</div>
</template>

<script>
	// @ is an alias to /src
	import HeroSection from "@/views/HeroSection.vue";
	import Tecnologias from "@/views/Tecnologias.vue";

	export default {
		name: "Home",
		components: {
			HeroSection,
			Tecnologias,
		},
	};
</script>
