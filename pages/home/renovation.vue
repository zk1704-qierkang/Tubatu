<template>
	<view class="content">
		<view>
			<mehaotian></mehaotian>
			<view class="tu">
				<view class="tv">
					<image src="../../static/imgs/tehui.png"></image>
					<view class="wz">装企特惠</view>
				</view>
				<view class="tv">
					<image src="../../static/imgs/quanwudingzhi.png" class="dingzhi"></image>
					<view class="wz">全屋定制</view>
				</view>
				<view class="tv">
					<image src="../../static/imgs/liangfang.png"></image>
					<view class="wz">上门量房</view>
				</view>
				<view class="tv">
					<image src="../../static/imgs/shangcheng.png"></image>
					<view class="wz">家居商城</view>
				</view>
			</view>
			<wlp></wlp>
			<view class="tj">
				<view class="yi">
					<view class="zi">
						<text>周口宏信装饰</text>
					</view>
					<view class="zix">
						<text class="an">案例：4</text>
						<text class="g">|</text>
						<text class="gong">工地：3</text>
					</view>
					<view class="img">
						<image src="../../static/imgs/t1.jpg"></image>
						<image src="../../static/imgs/t2.jpg"></image>
						<image src="../../static/imgs/t3.jpg"></image>
					</view>
				</view>
			</view>
			<view class="tj2">
				<view class="er">
					<view class="zi">
						<text>周口宏信装饰</text>
					</view>
					<view class="zix">
						<text class="an">案例：4</text>
						<text class="g">|</text>
						<text class="gong">工地：3</text>
					</view>
					<view class="img">
						<image src="../../static/imgs/t4.jpg"></image>
						<image src="../../static/imgs/t5.jpg"></image>
						<image src="../../static/imgs/t6.jpg"></image>
					</view>
				</view>
				<view class="tj2">
					<view class="er">
						<view class="zi">
							<text>周口宏信装饰</text>
						</view>
						<view class="zix">
							<text class="an">案例：4</text>
							<text class="g">|</text>
							<text class="gong">工地：3</text>
						</view>
						<view class="img">
							<image src="../../static/imgs/t7.jpg"></image>
							<image src="../../static/imgs/t8.jpg"></image>
							<image src="../../static/imgs/t9.jpg"></image>
						</view>
					</view>
				</view>
			</view>
		</view>
	</view>
</template>

<script>
	import wlp from "../../components/wlp-swiper-banner2/wlp-swiper-banner.vue"
	import mehaotian from "../../components/mehaotian-search/mehaotian-search.vue"
	export default {
		components: {wlp,mehaotian},
		data() {
			return {
				
			}
		},
		mounted() {
			
		},
		methods:{
			
		}
	}
</script>

<style>
	@import "../../static/css/renovation.css";
</style>
