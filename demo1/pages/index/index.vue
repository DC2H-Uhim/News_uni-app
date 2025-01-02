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
		height: 1334rpx;//高满屏
		background: green;
	}
}
</style>
