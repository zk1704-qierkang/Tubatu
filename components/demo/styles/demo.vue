<template>
	<view class="content">
		
		
		<view>
			<wuc-tab :tab-list="tabList" :tabCur.sync="TabCur" textFlex='true' @change="tabChange" class="a"></wuc-tab>
			<view >
				<view v-show="TabCur === 0" >
					<view class="fn">
						<image src="../../../static/imgs/14.jpg"></image>
					</view>
				</view>
				<view v-show="TabCur === 1" >
					<view class="fn">
						<image src="../../../static/imgs/15.jpg"></image>
					</view>
				</view>
				<view v-show="TabCur === 2" >
					<view class="fn">
						<image src="../../../static/imgs/16.jpg"></image>
					</view>
				</view>
				<view v-show="TabCur === 3" >
					<view class="fn">
						<image src="../../../static/imgs/17.jpg"></image>
					</view>
				</view>
				<view v-show="TabCur === 4" >
					<view class="fn">
						<image src="../../../static/imgs/18.jpg"></image>
					</view>
				</view>
				<view v-show="TabCur === 5" >
					<view class="fn">
						<image src="../../../static/imgs/19.jpg"></image>
					</view>
				</view>
				<view v-show="TabCur === 6" >
					<view class="fn">
						<image src="../../../static/imgs/7.jpg"></image>
					</view>
				</view>
				
			</view>
		</view>
		
	</view>
</template>

<script>
	import WucTab from '@/components/wuc-tab/wuc-tab.vue';
	export default {
		components: {
			WucTab
		},
		data() {
			return {
				TabCur: 0,
				tabList: [{ name: '推荐' }, { name: '效果图' }, { name: '看方案' },
				{ name: '问答' }, { name: '攻略' }, { name: '日记' },
				{ name: '达人说' }],
			}
		},
		mounted() {
			
		},
		methods:{
			 tabChange(index) {
				this.TabCur = index;
			},
			fn(){
			
				uni.navigateTo({
					url:'shousuo'
				})
			}
			
		}
	}
</script>
<style>
	.q1{
		height: 60upx;
		width: 80%;
		border: #0081FF 1upx solid;
		margin-top: 20upx;
		margin-left: 40upx;
		border-radius: 30upx;
		padding-left: 30upx;
		font-size: 30upx;
	}
	.q2{
		margin-top: 10upx;
		color: #DDDDDD;
		display: inline-block;
		margin-left: 10upx;
	}
	.ww{
		height: 35upx;
		width: 35upx;
		margin-top: 5upx;
		display: inline-block;
	}
	.a{
		font-size: 20upx;
	}
	.fn{
		width: 100%;
		height: 400upx;
		border:1px solid #000;
	}
	.fn image{
		width: 100%;
		height: 400upx;
		border:1px solid #000;
	}
</style>
