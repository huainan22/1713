<template>
    <swiper :options="swiperOption">
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1710/f5/57137c621d75ba02.jpg_640x200_b984ddf7.jpg" />
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1609/15/630b82d932a3c402.jpg_640x200_862e836b.jpg" />
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1710/f5/57137c621d75ba02.jpg_640x200_b984ddf7.jpg" />
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1609/f3/52a119dbed871902.jpg_640x200_b4573df8.jpg">
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1710/f5/57137c621d75ba02.jpg_640x200_b984ddf7.jpg" />
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1609/c9/cacbf705c5417e02.jpg_640x200_99b2676a.jpg">
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="swiper-img-con">
                <img class="swiper-img" src="http://img1.qunarzz.com/piao/fusion/1710/f5/57137c621d75ba02.jpg_640x200_b984ddf7.jpg" />
            </div>
        </swiper-slide>
        <div class="home-swiper-pagination swiper-personalize"  slot="pagination"></div>
    </swiper>
</template>

<script>
    export default {
        data() {
            return {
                swiperOption: {
                    autoplay: 3000,
                    direction: 'horizontal',
                    autoHeight: true,
                    pagination: '.home-swiper-pagination',
                    bulletClass : 'home-bullet',
                    bulletActiveClass: 'home-bullet-active',
                    observeParents: true
                }
            }
        },
        components: {
            swiper,
            swiperSlide
        }
    }
</script>

<style>
    import { swiper,swiperSlide } from "vue-awesome-swiper";
    .swiper-img-con {
        width: 100%;
        height: 0;
        padding-bottom: 31.25%;
    }
    .swiper-img {
        width: 100%;
    }
    .swiper-container {
        position: relative;
    }
    .home-swiper-pagination, .swiper-pagination-bullets {
        position:absolute;
        bottom: 1.2rem;
        z-index: 99; 
        width: 100%;
        text-align:center;    
    }
    .home-bullet {
        display:inline-block;
        width: .13rem;
        height: .13rem;
        margin: 0 .06rem;
        border-radius: 50%;
        background:rgba(144, 144, 144, 0.5);  
    }
    .home-bullet-active {
        background: #fff;
    }
</style>