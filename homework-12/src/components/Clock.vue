<!-- Clock qism -->

<template>
	<div>
		<h1 class="text-4xl"></h1>
		{{ hour }}:{{ minutes }}:{{ seconds }}
	</div>
</template>

<script>
export default {
	data() {
		return {
			hour: '',
			minutes: '',
			seconds: '',
			intervalId: '',
		}
	},
	created() {
		this.getCurrentTime()
	},
	methods: {
		getCurrentTime() {
			this.intervalId = setInterval(() => {
				const date = new Date()
				this.hour = date.getHours().toString().padStart(2, 0)
				this.minutes = date.getMinutes().toString().padStart(2, 0)
				this.seconds = date.getSeconds().toString().padStart(2, 0)

				console.log('interval')
			}, 2000)
		},
	},
}
</script>

<style lang="scss" scoped></style>
