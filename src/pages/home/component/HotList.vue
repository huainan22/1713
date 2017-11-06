<template>
	<div class="hotlist">
		<div class="hotlist-title">
			<h2 class="holist-title-name">
				热销推荐
			</h2>
		</div>
		
		<ul class="hotlist-item" >
			<li class="hot-prod" v-for="list in lists" :key="list.id">
				<a href="">
					<div class="hotlist-pic">
						<img :src="list.img" alt="" class="hotlist-img">
					</div>
					<div class="hotlist-cntent">
						<p class="hotlist-fir">{{list.title}}</p>
						<p class="hotlist-sec">{{list.explain}}</p>
					</div>
					<div class="hotlist-price">
						￥<span class="price-num">{{list.price}}</span><span class="price-text">起</span>
					</div>
				</a>
			</li>
		</ul>
		<div class="moreproduct">
			<a href="">查看更多产品</a>
		</div>
	</div>

</template>

<script>
	import Vue from "vue";
	export default {
		data() {
			return {
				lists: [{
					img:"http://img1.qunarzz.com/sight/p0/1409/19/adca619faaab0898245dc4ec482b5722.jpg_140x140_80f63803.jpg",
					title: "故宫",
					explain: "东方宫殿建筑代表，世界宫殿建筑典范",
					price: 65,
					id: 1
				},{
					img:"http://img1.qunarzz.com/sight/p0/1708/2b/2b3b94de99c0a425a3.img.jpg_140x140_97813766.jpg",
					title: "八达岭长城",
					explain: "不到长城非好汉",
					price: 25,
					id: 2
				},{
					img:"http://img1.qunarzz.com/sight/p0/1505/d2/d274c92de14c93da.water.jpg_140x140_e20be8e0.jpg",
					title: "颐和园",
					explain: "保存完整的一座皇城行宫御苑",
					price: 1,
					id: 3
				},{
					img:"http://img1.qunarzz.com/sight/p0/1508/a5/4003f9dd7bebf61eccbf64046e26d487.water.jpg_140x140_b05eb1df.jpg",
					title: "欢乐谷",
					explain: "七大主题园区带你畅想北京欢乐谷",
					price: 11,
					id: 4
				},{
					img:"http://img1.qunarzz.com/sight/p0/1708/2b/2b6378fd3b2e1d86a3.img.jpg_140x140_eae81520.jpg",
					title: "慕天峪长城",
					explain: "秀美长城，关键是人少",
					price: 19.1,
					id: 5
				}]
			}				
		}	
	}
</script>

<style>
	.hotlist {
		width: 100%;
		color: #212121;
    		
	}
	.hotlist-title{
		height: .8rem;
		padding-left: .26rem;
		line-height: .8rem;
	}
	.holist-title-name{
		width: 2rem;
		overflow: hidden;
		white-space: nowrap;
	    text-overflow: ellipsis
	}
	#app {
		width: 100%;
	    min-height: 100%;
	    background: #f5f5f5; 
	}
	.hotlist-item {
		background: #fff;
	}
	.hot-prod {
		position: relative;
	    overflow: hidden;
	    height: 1.4rem;
	    padding: .24rem;
	    border-bottom: 1px solid #ccc;
	}
	.hotlist-pic {
		position: absolute;
	    top: .24rem;
	    left: .24rem;
	    width: 1.4rem;
    	height: 1.4rem;
	}
	.hotlist-img {
		width: 100%;
	}
	.hotlist-cntent {
		margin-left: 1.6rem;
	}
	.hotlist-fir {
		overflow: hidden;
	    margin-top: .04rem;
	    margin-bottom: .1rem;
	    color: #212121;
	    font-size: .3rem;
	    white-space: nowrap;
	    text-overflow: ellipsis
	}
	.hotlist-sec {
		overflow: hidden;
	    margin-bottom: .1rem;
	    height: .4rem;
	    line-height: .4rem;
	    color: #9e9e9e;
	    white-space: nowrap;
	    text-overflow: ellipsis;
	}
	.hotlist-price {
		margin-left: 1.6rem;
    	color: #ff8300;
	}
	.price-num {
		font-size: .36rem;
    	padding: 0 .04rem;
	}
	.price-text {
		color: #9e9e9e;
    	font-size: .24rem;
	}
	.moreproduct {
		height: .88rem;
	    color: #00afc7;
	    line-height: .88rem;
	    text-align: center;
	    background: #fff;
	}
</style>