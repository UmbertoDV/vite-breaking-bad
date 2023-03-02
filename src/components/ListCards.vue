<script>
import AppCard from "./AppCard.vue";
import axios from "axios";

export default {
	data() {
		return {
			cards: [],
			allFoundCards: 0,
		};
	},

	components: {
		AppCard,
	},

	created() {
		axios
			.get("https://db.ygoprodeck.com/api/v7/cardinfo.php?num=10&offset=0")
			.then((response) => {
				console.log(response);
				this.cards = response.data.data;
				// console.log(this.cards);
				this.allFoundCards = this.cards.length;
			});
	},
};
</script>

<template>
	<div class="container">
		<div class="cards-founds">
			<h5 class="my-0 p-4 fw-bold">Found {{ allFoundCards }} Cards</h5>
		</div>
		<div class="row row-cols-5 align-items-stretch">
			<AppCard v-for="(card, index) in cards" :card="card" :key="index" />
		</div>
	</div>
</template>

<style lang="scss" scoped>
//SCSS
@use "../assets/scss/partials/mixins" as *;

.container {
	padding: 50px;
	background-color: white;
	width: 100%;
	.cards-founds {
		background-color: #212529;
		width: 100%;
		color: white;
	}
}
</style>
