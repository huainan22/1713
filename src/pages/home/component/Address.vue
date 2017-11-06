<template>
	<div id="add">
		<div class="address">
			<a href="" class="address-left">
				<p class="address-word"><i class="iconfont icon-dingwei"></i>定位失败</p>
			</a>
			<a href="" class="address-right">
				<p class="address-word"><i class="iconfont icon-diqiu"></i>五折泡温泉</p>
			</a>
		</div>
		<div class="promotion">
			<a href="" class="promotion-left">
				<div class="promotion-left-word">
					<h2 class="promotion-title">精选温泉</h2>
					<p class="promotion-word">5折开泡</p>					
				</div>
				<img src="../../../app/images/add-img_03.jpg" alt="" class="promotion-img">
			</a>
			<a href="" class="promotion-right">
				<div class="promotion-right-word">
					<h2 class="promotion-title">金秋大促</h2>
					<p class="promotion-word">门票1元起</p>					
				</div>
				<img src="../../../app/images/add-img_06.jpg" alt="" class="promotion-img">
			</a>
		</div>
	</div>
</template>

<script>

</script>

<style scoped>
	.address {
		width: 100%;
		height: .98rem;
		text-align: center;
		line-height: .98rem;
		padding-bottom: .1rem;
	}
	.address .address-word {
		display: inline-block;
		width: 1.8rem;
		white-space: nowrap;
		overflow: hidden;
		text-overflow: ellipsis;
	}
	.address-left {
		float: left;
		width: 49.8%;
		height: .98rem;
		color: #212121;
		background: #fff;
	}
	.address-right {
		float: right;
		width: 49.8%;
		height: .98rem;
		color: #212121;
		background: #fff;
	}
	.promotion {
		height: 1.2rem;
	}
	.promotion-left {
		float: left;
		width: 49.8%;
		height: 1.2rem;
		background: #fff;
	}
	.promotion-right {
		float: right;
		width: 49.8%;
		height: 1.2rem;
		background: #fff;
	}
	.promotion .promotion-left-word,.promotion-right-word {
		float: left;
	}
	.promotion .promotion-img {
		margin-top:.08rem;
		margin-right: .19rem;
		float: right;
	}
	.promotion .promotion-title {
		width: 1.5rem;
		white-space: nowrap;
		overflow: hidden;
		text-overflow: ellipsis;
		margin:.16rem 0 .1rem .22rem;
		color: #fe0e0e;
	}
	.promotion .promotion-word {
		width: 1.2rem;
		white-space: nowrap;
		overflow: hidden;
		text-overflow: ellipsis;
		margin-left: .22rem;
		font-size: .12rem;
		color:#8d8d8d;
	}
</style>
