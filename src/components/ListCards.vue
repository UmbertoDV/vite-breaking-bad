<script>
import AppCard from "./AppCard.vue";
export default {
	data() {
		return {
			title: "Hello World",
		};
	},

	components: {
		AppCard,
	},
};
</script>

<template>
	<div
		class="container d-flex flex-column align-items-start justify-content-center"
	>
		<div class="cards-founds">
			<h5 class="my-0 p-4 fw-bold">Found 3 Cards</h5>
		</div>
		<div class="row row-cols-5 align-items-stretch g-3">
			<AppCard />
			<AppCard />
			<AppCard />
			<AppCard />
			<AppCard />
			<AppCard />
		</div>
	</div>
</template>

<style lang="scss" scoped>
//SCSS
@use "../assets/scss/partials/mixins" as *;

.container {
	padding: 50px;
	background-color: white;
	@include flex("vertical");
	.cards-founds {
		background-color: #212529;
		width: 100%;
		color: white;
	}
}
</style>
