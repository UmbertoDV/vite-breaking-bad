<script>
// import HelloWorld from './components/HelloWorld.vue'
export default {
	data() {
		return {
			title: "Hello World",
		};
	},

	// components:{
	//	 HelloWorld,
	// }
};
</script>

<template>
	<div class="text-center col d-flex flex-column py-3">
		<img src="https://images.ygoprodeck.com/images/cards/34541863.jpg" alt="" />
		<div class="testo py-2">
			<h2 class="my-2 fs-5">CELL BREEDIN</h2>
			<span class="my-1">ALIEN</span>
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
