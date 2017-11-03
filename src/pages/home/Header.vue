<template>
    <div class="header">
    	<a class="header-left"> <i class="iconfont icon-fanhui"></i> </a>

    	<div class="header-title">
    		<i class="iconfont icon-fangdajing"></i>
    			输入城市/景点/游玩主题 		
    	</div>
    	<div class="header-right">
    		<span class="nav-city">北京</span>
    	</div>
   	</div>
</template>

<script>
	export default {
	  
	}
</script>


<style scoped>
	.header{
		position: relative;
    	width: 100%;
    	height: .88rem;
    	background: #00bcd4;
    	text-align: center;
    	color: #fff;
	}
	.header-left{
    	float:left;
    	width: .4rem;
   	 	line-height: .88rem;
    	padding: 0 .2rem;
    	color: #fff;
   		font-size: .36rem;
    	text-align: left;
	}
	.header-title{
	    position: absolute;
	    top: .14rem;
	    left: .8rem;
	    right: 1.28rem;
	    line-height: .6rem;
	    background: #fff;
	    color: #ccc;
	    border-radius: .06rem;
	}
	.header-right {
		float: right;
		width: 1.28rem;
		line-height: .88rem;
	}
	.nav-city{
		float:left;
		width:.85rem;
		overflow:hidden;
		text-overflow: ellipsis;
		white-space: nowrap;	
	}
	.nav-city:after {
		position: absolute;
		top: .35rem;
	    right: .13rem; 
	    width: 0;
	    content: "";
		border-left: .15rem solid transparent;  
	    border-right: .15rem solid transparent;  
	    border-top: .155rem solid #fff;      
	}
	
	/*.icon-fangdajing{
		color:#000;
		font-size:.3rem;
	}*/
</style>