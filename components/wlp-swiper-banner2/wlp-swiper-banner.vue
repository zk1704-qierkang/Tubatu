<template>
    <view class="swiper" :style="{ 'padding-bottom': height + '%' }">
        <swiper
            class="swiper__main"
            autoplay="true"
            circular="true"
            interval="5000"
            duration="500"
            indicator-color="#ccc"
            indicator-active-color="#07bc91"
        >
            <block v-for="(item, index) in data" :key="index">
                <swiper-item class="swiper__cell" @tap="_click(index)">
                    <image class="swiper__img" :src="item" mode="aspectFill"></image>
                </swiper-item>
            </block>
        </swiper>
    </view>
</template>

<script>
export default {
    props: {
        data: {
            type: Array,
            default: function(e) {
                return ["../../static/imgs/1.jpg",
				"../../static/imgs/4.jpg",
				"../../static/imgs/5.jpg",
				"../../static/imgs/6.jpg",
				"../../static/imgs/7.jpg",
				"../../static/imgs/9.jpg"];
            }
        },
        height: { // 高宽百分比
            type: Number,
            default: function(e) {
                return 50;
            }
        }
    },
    methods: {
        _click: function(index) {
            this.$emit('click', index);
        },
    }
};
</script>

<style>
/* swiper宽高等比 */
.swiper{
    position: relative;
    width: 100%;
    padding-bottom: 66.67%;
	margin-top: 10upx;
}
.swiper__main{
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    width: 100%;
    height: 240upx;
	border-bottom: #F1F1F1 0.5upx solid;
}
.swiper__cell,.swiper__img{
    width: 94%;
    height: 200upx;
	border-radius:7px
}
</style>
