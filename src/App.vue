<script>
import AppHeader from "./components/AppHeader.vue";
import AppMain from "./components/AppMain.vue";

export default {
	data() {
		return {
			title: "",
		};
	},

	components: {
		AppHeader,
		AppMain,
	},
};
</script>

<template>
	<AppHeader />
	<AppMain></AppMain>
</template>

<style lang="scss">
//SCSS
@use "./assets/scss/style.scss";
</style>
