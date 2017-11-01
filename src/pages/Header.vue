<template>
    <div class="header">
    	<a class="header-left"> < </a>
    	<div class="header-title">
    		<span class="single-line">输入城市/景点/游玩主题</span>  		
    	</div>
    	<div class="header-right" mp-role="right">
    		<span class="nav-city">北京</span>
    		<span class="trangle-down"></span>
    	</div>
   	</div>
</template>

<script>
export default {
  name: 'Header',
  data () {
    return {
      msg: 'header'
    }
  }
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
	.trangle-down {
		float:right;
		margin-right:.2rem;
		margin-top: .35rem;
		width: 0;
		height: 0;
		border-left: .12rem solid transparent;
		border-right: .12rem solid transparent;
		border-top: .2rem solid #fff;
	}
</style>