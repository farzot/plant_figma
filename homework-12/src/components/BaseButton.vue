<!-- Button qism -->

<template>
	<div>
		<button class="py-3 px-6 bg-orange-500 rounded text-white">
			<Icon icon="mdi-user" class="tex-red-500" />
			<slot />
		</button>
	</div>
</template>

<script>
import { Icon } from '@iconify/vue'
export default {
	components: { Icon },
}
</script>

<style lang="scss" scoped></style>
