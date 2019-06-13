<template>
	<view class="content">
		<view>
			<mehaotian></mehaotian>
			<wlp></wlp>
			<view class="daohang">
				<view class="d1">
					<image src="../../static/imgs/11.jpg"></image>
					<view>算报价</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/10.jpg"></image>
					<view>找设计</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/12.jpg"></image>
					<view>装修公司</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/13.jpg"></image>
					<view>审核报价</view>
				</view>
			</view>
			<view class="zhong">
				<view class="zuo">
					<image src="../../static/imgs/2.jpg"></image>
				</view>
				<view class="youshang">
					<image src="../../static/imgs/3.jpg"></image>
				</view>
				<view class="youxia">
					<image src="../../static/imgs/8.jpg"></image>
				</view>
			</view>
		</view>
		<view>
			<demo></demo>
		</view>
	</view>
</template>

<script>
	import wlp from "../../components/wlp-swiper-banner/wlp-swiper-banner.vue"
	import mehaotian from "../../components/mehaotian-search/mehaotian-search.vue"
	import demo from "../../components/demo/styles/demo.vue"
	export default {
		components: {wlp,mehaotian,demo},
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
	@import "../../static/css/sy.css";
</style>
