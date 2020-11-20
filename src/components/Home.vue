<template>
	<Page actionBarHidden="true">
		<StackLayout backgroundColor="#191C21">
			<ScrollView>
				<StackLayout class="home-panel">
					<Label textWrap="true" text="Play with NativeScript!"
						   class="h2 description-label" />
					<Label textWrap="true"
						   text="Write code in the editor or drag and drop components to build a NativeScript mobile application."
						   class="h2 description-label" />
					<Label textWrap="true"
						   text="Scan the QR code with your mobile device and watch the changes sync live while you play with the code."
						   class="h2 description-label" />
				</StackLayout>
			</ScrollView>
			<StackLayout class="input" color="#ffffff" padding="10 20">
				<Label textWrap="true" text="123,456,789"
					   horizontalAlignment="right" fontSize="34" />
			</StackLayout>
			<GridLayout class="keypad" columns="*, *, *, *"
						rows="*, *, *, *, *" backgroundColor="#252932">
				<Label class="key" text="c" row="0" col="0" touch="keyTouch"
					   horizontalAlignment="center" color="#175a62"
					   verticalAlignment="center" fontSize="28" />
				<Label class="key" text="+/-" row="0" col="1"
					   horizontalAlignment="center" color="#175a62"
					   verticalAlignment="center" fontSize="22" />
				<Label class="key" text="%" row="0" col="2"
					   horizontalAlignment="center" color="#175a62"
					   verticalAlignment="center" fontSize="22" />
				<Label class="key" text="÷" row="0" col="3"
					   horizontalAlignment="center" color="#fe7771"
					   verticalAlignment="center" fontSize="34" />
				<Label class="key" text="7" row="1" col="0"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="8" row="1" col="1"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="9" row="1" col="2"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="×" row="1" col="3"
					   horizontalAlignment="center" color="#fe7771"
					   verticalAlignment="center" fontSize="34" />
				<Label class="key" text="4" row="2" col="0"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="5" row="2" col="1"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="6" row="2" col="2"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="-" row="2" col="3"
					   horizontalAlignment="center" color="#fe7771"
					   verticalAlignment="center" fontSize="34" />
				<Label class="key" text="1" row="3" col="0"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="2" row="3" col="1"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="3" row="3" col="2"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="+" row="3" col="3"
					   horizontalAlignment="center" color="#fe7771"
					   verticalAlignment="center" fontSize="34" />
				<Label class="key" text="0" row="4" col="1"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="." row="4" col="2"
					   horizontalAlignment="center" verticalAlignment="center"
					   fontSize="20" />
				<Label class="key" text="=" row="4" col="3"
					   horizontalAlignment="center" color="#fe7771"
					   verticalAlignment="center" fontSize="34" />
			</GridLayout>
		</StackLayout>
	</Page>
</template>

<script>
export default {
	data() {
		return {};
	},
	methods: {
		keyTouch(args) {
			console.log("Touch arguments: ", args);
		}
	}
};
</script>

<style scoped>
ScrollView {
	height: 30%;
}

.keypad {
	color: #f7f7f7;
	height: 70%;
}

.key:active {
	backgroundColor: #5c5e61;
}
</style>