<script>
// import HelloWorld from './components/HelloWorld.vue'
export default {
	data() {
		return {};
	},

	props: {
		card: Object,
		key: Number,
	},
	// components:{
	//	 HelloWorld,
	// }
};
</script>

<template>
	<div class="text-center col d-flex flex-column py-3">
		<img :src="card.card_images[0].image_url" alt="" />
		<div class="testo py-2">
			<h2 class="my-2 fs-5">{{ card.name }}</h2>
			<span class="my-1">{{ card.archetype }}</span>
		</div>
	</div>
</template>

<style lang="scss" scoped>
.testo {
	background-color: #d48f3a;
	display: flex;
	flex-grow: 1;
	flex-direction: column;
	justify-content: center;
	h2 {
		color: white;
	}
	span {
		font-weight: bold;
	}
}
//SCSS
</style>
