<template>
	<view>

	</view>
</template>

<script>
	export default {
		data() {
			return {

			}
		},
		onLoad() {
			// #ifdef APP-PLUS
			// this.playVideo()
			uni.$on('drawer-page', (data) => {
				uni.showToast({
					title: '点击了第' + data + '项',
					icon: "none"
				});
			})
			// #endif
		},
		onUnload() {
			uni.$off('drawer-page')
		},
		methods: {

		}
	}
</script>

<style>

</style>
