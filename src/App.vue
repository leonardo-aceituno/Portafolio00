<template>
	<div id="app">
		<Nav />
		<!-- <div id="nav">
			<router-link to="/">Home</router-link> |
			<router-link to="/about">About</router-link>
		</div> -->
		<router-view />
	</div>
</template>

<script>
	import Nav from "@/components/Nav";

	export default {
		components: { Nav },
	};
</script>


<style>
	@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@300;400;700;800;900&display=swap");

	#app {
		font-family: "Montserrat", sans-serif;
		/* text-align: center; */
		color: rgb(56, 56, 56);
	}

	.size46 {
		font-size: 2.875rem;
	}

	.size20 {
		font-size: 1.25rem;
	}

	.font-black {
		font-weight: 900;
	}

	.font-bold {
		font-weight: 700;
	}

	#nav {
		padding: 30px;
	}

	#nav a {
		font-weight: bold;
		color: #2c3e50;
	}

	#nav a.router-link-exact-active {
		color: #42b983;
	}
</style>
