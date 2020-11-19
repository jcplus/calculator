<template>
	<Page>
		<ActionBar title="Calculator App"/>
		<GridLayout columns="*, *, *" rows="*, *, *">
			<CalculatorKey class="key" :text="7" row="0" col="0"></CalculatorKey>
			<CalculatorKey class="key" :text="8" row="0" col="1"></CalculatorKey>
			<CalculatorKey class="key" :text="9" row="0" col="2"></CalculatorKey>
		</GridLayout>
	</Page>
</template>

<script>
import CalculatorKey from './CalculatorKey'

export default {
	components: {
		'CalculatorKey': CalculatorKey
	},
	data() {
		return {
			msg: 'Hello World!'
		}
	}
}
</script>

<style scoped>
ActionBar {
	background-color: #53ba82;
	color: #ffffff;
}

.key {
	margin: 0;
}
</style>
