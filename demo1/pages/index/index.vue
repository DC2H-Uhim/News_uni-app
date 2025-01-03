<template>
	<!-- Vue2要求仅有唯一的一个根标签view -->
	<!-- div,h1,h2这些标签的使用仅适用于H5页面的使用 -->
	<!--<div class="box">
		<h1>uni-app<span class="row">零基础</span>入门</h1>
		<view class="">
			从基础到进阶
		</view>
		<h2>标题二加粗<i>标签</i></h2>
	</div> -->
	<view class="out">
		<view class="box">
		</view>
		<view class="block">
		</view>
		<!-- 内置icon组件 无法满足需求，后续会使用第三方组件 -->
		<icon type="success" size="26"/>
		<!-- view是块标签替换div，text是行标签替换span -->
		<view>uni-app</view>
		<view>web前端开发</view>
		<text user-select selectable>node.js</text>
		<text space="emsp" decode>vue.  &Equilibrium;  js</text>
		<!-- 滑块盒子：可滚动视图区域滑动 -->
		<scroll-view class="scroll" scroll-x scroll-y>
			<view class="group">
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
				<view class="item">
					111
				</view>
			</view>
		</scroll-view>
		<!-- 轮播器：页面滑动 -->
		<swiper indicator-dots="true" autoplay interval="3000" duration="1000">
			<swiper-item class="item" style="background: red;">1111</swiper-item>
			<swiper-item class="item" style="background: yellow;">2222</swiper-item>
			<swiper-item class="item" style="background: skyblue;">3333</swiper-item>
			<swiper-item class="item" style="background: green;">4444</swiper-item>
		</swiper>
	</view>
</template>

<script>
	export default {

	}
</script>

<style lang="scss">//css的加长版，可以类似嵌套一样的使用
// .box{
// 	height: 100px;
// 	background: pink;
// 	h1{
// 		font-size: 40px;
// 		color: red;
// 		.row{
// 			font-style: italic;
// 		}
// 	}
// }
.out{
	.box{//rpx:响应式单位
		width: 200px;
		height: 200px;
		background: pink;
	}
	.block{
		width: 750rpx;//宽满屏
		height: 200rpx;//1334rpx高满屏
		background: green;
	}
}
.scroll{
	border: 1px solid red;
	box-sizing: border-box;//内边框满屏
	height: 220rpx;
	.group{
		white-space: nowrap;//不换行
		.item{
			width: 220rpx;
			height: 220rpx;
			height: 100rpx;
			background: royalblue;
			display: inline-block;//行级块元素
			margin-right: 10rpx;
		}
	}
}
</style>
