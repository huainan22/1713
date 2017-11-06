<template>
    <swiper :options="swiperOption">
        <swiper-slide v-for="item in swiperInfo" :key="item.id">
            <router-link :to="item.link">
                <div class="swiper-img-con">
                    <img class="swiper-img" :src="item.imgUrl">
                </div>
            </router-link>
        </swiper-slide>
        <div class="home-swiper-pagination"  slot="pagination"></div>
    </swiper>
</template>

<script>
    import { swiper,swiperSlide } from "vue-awesome-swiper";
    export default {
        props: ['swiperInfo'],
        data() {
            return {
                swiperOption: {
                    autoplay: 3000,
                    direction: 'horizontal',
                    autoHeight: true,
                    pagination: '.home-swiper-pagination',
                    bulletClass : 'home-swiper-bullet',
                    bulletActiveClass: 'home-swiper-bullet-active',
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
    .home-swiper-pagination, .swiper-pagination-bullets {
        width: 100%;
        z-index: 99;
        text-align: center;
        position: absolute;
        bottom: 1.2rem;  
    }
    .home-swiper-bullet {
        display: inline-block;
        width: .13rem;
        height: .13rem;
        margin: 0 .06rem;
        border-radius: 50%;
        background: rgba(144, 144, 144, 0.5);  
    }
    .home-swiper-bullet-active {
        background: #fff;
    }
</style>

<style scoped> 
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
</style>