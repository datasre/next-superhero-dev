<template>
	<view >
		<swiper :indicator-dots="true" :autoplay="true" class="catousel">
			<swiper-item>
				<image src="../../static/carousel/batmanvssuperman.png" class="catousel" ></image>
			</swiper-item>
			<swiper-item>
				<image src="../../static/carousel/spiderman.png" class="catousel"></image>
			</swiper-item>
		</swiper>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				title: 'Hello'
			}
		},
		onLoad() {
			uni.request({
			    url: 'https://www.example.com/request', //仅为示例，并非真实接口地址。
			    success: (res) => {
			        console.log(res.data);
			        this.text = 'request success';
			    }
			});
		},
		methods: {

		}
	}
</script>

<style>
	@import url("./index.css");
</style>
