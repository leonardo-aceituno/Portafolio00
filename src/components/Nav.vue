<template>
	<div>
		<b-navbar toggleable="lg" type="dark" variant="dark" class="fixed-top">
			<b-container>
				<b-navbar-toggle target="navbar-toggle-collapse">
					<template #default="{ expanded }">
						<b-icon v-if="expanded" icon="chevron-bar-up"></b-icon>
						<b-icon v-else icon="chevron-bar-down"></b-icon>
					</template>
				</b-navbar-toggle>

				<b-navbar-brand href="#">Portafolio</b-navbar-brand>

				<b-collapse id="navbar-toggle-collapse" is-nav>
					<b-navbar-nav class="ms-auto" fill>
						<b-nav-item class="nav-item" href="/">Home</b-nav-item>
						<b-nav-item class="nav-item" href="#tecnologias"
							>Tecnologías</b-nav-item
						>
					</b-navbar-nav>
				</b-collapse>
			</b-container>
		</b-navbar>
	</div>
</template>

<script>
	export default {
		methods: {
			scrollInto(elementId) {
				const section = document.querySelector(`#${elementId}`);
				section.scrollIntoView({
					behavior: "smooth",
				});
			},
		},
	};
</script>

<style scoped>
	.nav-item:hover {
		text-decoration-line: underline;
		text-decoration-thickness: 15%;
		text-underline-offset: 6px;
		
	}
</style>