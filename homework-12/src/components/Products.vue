<!-- Product qismi -->

<template>
	<div>
		<div class="flex justity-between item-center gap-x-8">
			<h2>All Plants</h2>
			<h2>New Arrivals</h2>
			<h2>Sale</h2>
		</div>
		<!-- <div class="grid grid-cols-3">
			<!-- <ProductCard v-for="item in 9" /> -->
			<!-- <ProductCard /> -->
		<!-- </div> --> 
		
	</div>
</template>
<script>
import ProductCard from './ProductCard.vue'
export default {
	components: {
		ProductCard,
	},
}
</script>
<style lang="scss" scoped></style>
