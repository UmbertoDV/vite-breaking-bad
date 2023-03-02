<script>
import ListCards from "./ListCards.vue";
import ChoiceRace from "./ChoiceRace.vue";

export default {
	data() {
		return {
			title: "Hello World",
		};
	},
	components: {
		ListCards,
		ChoiceRace,
	},
};
</script>

<template>
	<main>
		<ChoiceRace></ChoiceRace>
		<ListCards />
	</main>
</template>

<style lang="scss" scoped>
//SCSS
@use "../assets/scss/partials/mixins" as *;
</style>
