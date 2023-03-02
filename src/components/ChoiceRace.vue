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
	<div class="container py-4 px-0">
		<select class="form-select form-select-lg" name="" id="">
			<option selected>All</option>
			<option value="">New Delhi</option>
			<option value="">Istanbul</option>
			<option value="">Jakarta</option>
		</select>
	</div>
</template>

<style lang="scss" scoped>
//SCSS
.form-select {
	width: 200px;
}
</style>
