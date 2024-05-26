<script>
import { Icon } from '@iconify/vue/dist/iconify.js'
import BaseButton from './components/BaseButton.vue'
import BaseFilter from './components/BaseFilter.vue'
import Clock from './components/Clock.vue'
import Header from './components/Header.vue'
import Intro from './components/Intro.vue'
import OurBlog from './components/OurBlog.vue'
import ProductCard from './components/ProductCard.vue'
import Products from './components/Products.vue'
import SummerCastes from './components/SummerCastes.vue'

export default {
	components: {
		Header,
		BaseButton,
		BaseFilter,
		ProductCard,
		Products,
		Icon,
		Clock,
		Intro,
		SummerCastes,
		OurBlog,
	},
	data() {
		return {}
	},
}
</script>

<template>
	<div>
		<div class="container">
			<Header />
			<Intro class="mb-[26px]" />
			<div class="m-full flex gap-x-20 mb-[219px]">
				<BaseFilter class="w-1/3" />
				<ProductCard class="w-3/4" />
			</div>
			<SummerCastes class="mb-[138px]" />
			<OurBlog />
		</div>
	</div>
</template>

<style scoped>
.grid {
	display: grid;
	grid-template-columns: repeat(
		4,
		1fr
	); /* Adjust the number of columns as needed */
	gap: 16px; /* Adjust the gap between grid items */
}
.col-span-3 {
	grid-column: span 3;
}
.read-the-docs {
	color: #888;
}
</style>
