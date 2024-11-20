<template>
		<swiper>
			<swiper-item v-for="pic of pics" :key="pic.id">
				<image :src="pic.url" class="banner"></image>
			</swiper-item>
		</swiper>
</template>

<script>
	export default {
		data() {
			let pics = [
					{ id: '1', url: "https://pcapi-xiaotuxian-front-devtest.itheima.net/miniapp/uploads/goods_preview_1.jpg" },
					{ id: '2', url: "https://pcapi-xiaotuxian-front-devtest.itheima.net/miniapp/uploads/goods_preview_2.jpg" },
					{ id: '3', url: "https://pcapi-xiaotuxian-front-devtest.itheima.net/miniapp/uploads/goods_preview_3.jpg" },
					{ id: '4', url: "https://pcapi-xiaotuxian-front-devtest.itheima.net/miniapp/uploads/goods_preview_4.jpg" },
					{ id: '5', url: "https://pcapi-xiaotuxian-front-devtest.itheima.net/miniapp/uploads/goods_preview_5.jpg" },
				];
			return {
				pics
			}
		},
		onLoad() {

		},
		methods: {

		}
	}
</script>

<style>
	.banner{
		width: 750rpx;
		height: 750rpx;
	}


</style>
