<template>
	<div id="app">
		<section class="hero is-dark shadow">
			<div class="hero-head">
				<navbar/>
			</div>
		</section>

		<div class="container">
			<router-view/>
		</div>
	</div>
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
	name: 'App',
	components: { Navbar }
};
</script>

<style lang="scss">
    $dark: #2C2F33;

    html,
    body {
        background-color: $dark !important;
        color: white !important;
    }

    .shadow {
        box-shadow: 5px 5px 20px rgba(0, 0, 0, 0.2);
    }
</style>
