<template>
	<Button class="calc-key" :text="text"></Button>
</template>

<script>
export default {
	props: {
		text: {
			default: '',
			type: Number|String
		}
	},
	data() {
		return {
		}
	}
}
</script>