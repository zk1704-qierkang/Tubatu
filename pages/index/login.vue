<template>
	<view class="content">
		<view>
			<view class="image">
				<image src="../../static/imgs/logo.jpg"></image>
			</view>
			<view>
				<view class="a">
					<input placeholder="请输入用户名" v-model="username"/>
				</view>
				<view class="aa">
					<input type="password" placeholder="请输入密码" v-model="password"/>
				</view>
				<view><uni-icon type="eye" size="20"></uni-icon></view>
				<view class="d">
					<text class="text" @click="fn">登录</text>
				</view>
			</view>
		</view>
		
	</view>
</template>

<script>
	export default {
		data() {
			return {
				username:"",
				password:""
			}
		},
		mounted() {
			
		},
		methods:{
				fn(){
					uni.request({
						url: this.url+'baseUser/login', //仅为示例，并非真实接口地址。
						data: {
							username: this.username,
							password: this.password
						},
						header: {
							'custom-header': 'hello' //自定义请求头信息
						},
						success: (res) => {
							if(res.data){
								uni.showToast({
									title: '成功',
									duration: 2000
								});
								uni.setStorage({
									key:'baseUser',
									data:res.data
								})
								uni.switchTab({
									url:"../home/sy"
								})
								console.log(res.data)
							}else{
								uni.showToast({
									title: '登入失败',
									duration: 2000
								});
								console.log(res.data)
							}
			
						}
					});
				}
			}
		}
</script>

<style>
	@import "../../static/css/login.css";
</style>
