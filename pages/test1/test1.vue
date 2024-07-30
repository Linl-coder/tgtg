<template>
 	<div>
 		<zjw-GoogleMap :markers="markers" style="width:750rpx;height:400rpx" :allbase64img="allbase64img"
 			:location="position" :scale="scale"></zjw-GoogleMap>
 	</div>
 </template>

 <script>
 	export default {
		name:"zjw-GoogleMap",
 		data() {
 			return {
 				allbase64img: "", // marker图标，base64格式
 				scale: 11, // 最大不超过17,
 				position: "-33.88790967887629,151.18823157", //格式为：纬度,经度,中间用英文逗号隔开。
 				markers: [{
 						"longitude": "34.25368318660438",
 						"latitude": "108.9836931296498",
 						"content": "兴庆公园",
 						"msg": "11111" // 点击marker之后，会返回msg。这个参数可以不传，不传的时候，msg返回的是marker的id
 					},
 					{
 						"longitude": "34.21273880031796",
 						"latitude": "108.97495355954523",
 						"content": "大唐芙蓉园",
 						"msg": "22222"
 					}
 				]
 			}
 		},

 	}
 </script>
