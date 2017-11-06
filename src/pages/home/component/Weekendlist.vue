<template>
	<div class="weekendList">
		<h2 class="list-title">周末去哪儿</h2>
		<ul class="list">
			<li class="list-item" v-for="list in lists" >
				<div class="img-mark">
					<img class="list-Img" :src="list.src" alt="">
				</div>
				<div class="list-con">
					<p class="list-name">{{list.name}}</p>
					<p class="list-article">{{list.article}}</p>
				</div>
			</li>
		</ul>
	</div>
</template>

<script>
	export default {

	

		data() {
		return	{		
			lists:[{
					id:1,
					src: "http://img1.qunarzz.com/sight/source/1510/6e/1ea71e2f04e.jpg_r_640x214_aa6f091d.jpg",
					name: "北京温泉排行榜",
					article: "细数北京温泉，温暖你的冬天"
				},{
					id:2,
					src: "http://img1.qunarzz.com/sight/source/1505/9e/21df651e19af5d.jpg_r_640x214_3ea5bb38.jpg",
					name: "寻找北京的皇城范儿",
					article: "数百年的宫廷庙宇，至今依旧威严霸气"
				},{
					id:3,
					src: "http://img1.qunarzz.com/sight/source/1505/aa/7baaf8a851d221.jpg_r_640x214_1431200f.jpg",
					name: "北京必游TOP10",
					article: "来北京必去的景点非这些地方莫属"
				},{
					id:4,
					src: "http://img1.qunarzz.com/sight/source/1509/81/0412da9c4db66a.jpg_r_640x214_8e23871e.jpg",
					name: "登高望远秋色佳",
					article: "山顶满眼彩色，此情此景醉了"
				},{
					id:5,
					src: "http://img1.qunarzz.com/sight/source/1509/28/1bb74b851279e6.jpg_r_640x214_64ebf0ee.jpg",
					name: "秋高气爽去礼佛",
					article: "秋风伴着美妙经声，品尝秋的另一番滋味"
				}]
			}	
		}
	}
</script>

<style scoped>
	.weekendList{
		background: #f5f5f5
	}

	.list-title {
		
		line-height: .8rem;
		padding-left: .26rem;
		color: #212121;
	}

	.list-item{
		margin-bottom: .1rem;
	}

	.img-mark {
		width: 100%;
		height: 0;
		padding-bottom: 38%;
	}

	.list-Img {
		width: 100%;
	}

	.list-con {
		padding: .14rem .2rem .2rem .2rem;
		background: #fff;
	}

	.list-name {
		line-height: .48rem;
		font-size: .28rem;
		color: #212121;	
	}

	.list-article {
		line-height: .42rem;
   		font-size: .24rem;
   		color: #616161;	
	}

	
</style>
