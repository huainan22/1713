<template>
	<header class="header">
		<a class="header-left">
			<i class="iconfont icon-fanhui"></i>
		</a>
		<div class="header-title" >
			<i class="iconfont icon-fangdajing"></i>
			输入城市/景点/游玩主题
		</div>
		<div class="header-right">
			<span class="nav-city">北京</span>
		</div>
	</header>
</template>

<script>

	export default {

	}

</script>

<style scoped>
	.header {
	    position: relative;
	    width: 100%;
	    height: .88rem;
	    background: #00bcd4;
	    text-align: center;
	    color: #fff;
	}
	.header-left {
		float:left;
	    width: .4rem;
	    line-height: .88rem;
	    padding: 0 .2rem;
	    font-size: .36rem;
	    text-align: left;
	    color: #fff;
	}
	.header-title {
	    position: absolute;
	    top: .14rem;
	    left: .8rem;
	    right: 1.28rem;
	    line-height: .6rem;
	    background: #fff;
	    color: #ccc;
	    border-radius: .06rem;
	    padding-left: .15rem;
	    text-align: left;
	}
	.header-right {
		float: right;
		width: 1.28rem;
		line-height: .88rem;
		text-align: left;
	}

	.nav-city {
		margin-left: .2rem;
	}

	.nav-city:after {
		border-left: .15rem solid transparent;  
	    border-right: .15rem solid transparent;  
	    border-top: .155rem solid #fff;  
	    content: "";  
	    position: absolute;      
	    width: 0;
	    top: .35rem;
	    right: .13rem;  
	}
</style>
