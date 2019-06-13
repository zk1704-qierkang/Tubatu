<template>
	<view class="center">
		<view class="logo" @click="goLogin" :hover-class="!login ? 'logo-hover' : ''">
			<image class="logo-img" :src="login ? uerInfo.avatarUrl :avatarUrl"></image>
			<view class="logo-title">
				<text class="uer-name" style="color: #000000;">Hi，{{login ? uerInfo.name : '您未登录'}}</text>
				<text class="go-login navigat-arrow" style="color: #000000;" v-if="!login">&#xe65e;</text>
			</view>
			<!-- <view class="shuju">
				<view>0</view>
				<view>发布</view>
			</view> -->
		</view>
		
		<view class="center-list">
			<text class="my">我的家</text>
			<view class="but">
				<button>立即享受专享服务</button>
			</view>
			<view class="bx">
				<text>预约量房</text>
				<text class="te">|</text>
				<text>免费设计</text>
				<text class="te">|</text>
				<text>装修报价</text>
			</view>
		</view>
		<view class="center-list">
			<text class="my">常用工具</text>
			<view class="ds">
				<view class="d1">
					<image src="../../static/imgs/fangwu1.png"></image>
					<view>企业定制</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/baogao.png"></image>
					<view>量房报告</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/qianbao.png"></image>
					<view>钱包</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/youhuiquan.png"></image>
					<view>优惠券</view>
				</view>
			</view>
			<view class="dx">
				<view class="d1">
					<image src="../../static/imgs/lipin.png"></image>
					<view class="sb">礼品</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/jizhang.png"></image>
					<view>装修记录</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/jisuanqi.png"></image>
					<view>计算器</view>
				</view>
				<view class="d1">
					<image src="../../static/imgs/rili.png"></image>
					<view class="sb">黄历</view>
				</view>
			</view>
			
		</view>
		<view class="center-list">
			<text class="my2">第三方服务</text>
				<view class="ds2">
					<view class="d2">
						<image src="../../static/imgs/shangcheng.png"></image>
						<view>家居商城</view>
					</view>
					<view class="d2">
						<image src="../../static/imgs/jinrongfuwu.png"></image>
						<view>金融服务</view>
					</view>
					<view class="d2">
						<image src="../../static/imgs/ying.png"></image>
						<view>赢万元现金</view>
					</view>
					<view class="d2">
						<image src="../../static/imgs/fangong.png"></image>
						<view>装修返工</view>
					</view>
				</view>
				<view class="dx2">
					<view class="d2">
						<image src="../../static/imgs/shaitu.png"></image>
						<view>装修咨询</view>
					</view>
					<view class="d2">
						<image src="../../static/imgs/ce.png"></image>
						<view>预算报价</view>
			</view>
		</view>
	</view>
	</view>
</template>

<script>
	export default {
		data() {
			return {
				login: false,
				avatarUrl: "../../static/imgs/person.png",
				uerInfo: {}
			}
		},
		methods: {
			goLogin() {
				if (!this.login) {
					console.log("点击前往登录")
				}
			}
		}
	}
</script>

<style>
	@import "../uni-center/center.css";
</style>