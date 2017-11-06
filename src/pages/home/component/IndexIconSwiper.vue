<template>
    <swiper :options="swiperOption" :not-next-tick="notNextTick" ref="mySwiper" class="index-icon-swiper">
        <swiper-slide>
            <div class="index-icon-wrap">
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/54/ace00878a52d9702.png" alt="">
                        <p class="index-icon-item">景点门票</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/35/2640cab202c41b02.png" alt="">
                        <p class="index-icon-item">动植物园</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/45/676b67d7078abc02.png" alt="">
                        <p class="index-icon-item">故宫</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/a9/ffc620dbda9b9c02.png" alt="">
                        <p class="index-icon-item">一日游</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/59/569d3c096e542502.png" alt="">
                        <p class="index-icon-item">必游榜单</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/6d/ee9eb965690ce402.png" alt="">
                        <p class="index-icon-item">秋色美</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/d0/e09575e66f4aa402.png" alt="">
                        <p class="index-icon-item">游乐场</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1710/a6/83f636bd75ae6302.png" alt="">
                        <p class="index-icon-item">泡温泉</p>
                    </a>
                </div>
            </div>
        </swiper-slide>
        <swiper-slide>
            <div class="index-icon-wrap">
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/54/ace00878a52d9702.png" alt="">
                        <p class="index-icon-item">景点门票</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1710/a6/83f636bd75ae6302.png" alt="">
                        <p class="index-icon-item">旅游团购</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/d0/e09575e66f4aa402.png" alt="">
                        <p class="index-icon-item">自由行</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/6d/ee9eb965690ce402.png" alt="">
                        <p class="index-icon-item">周边短途</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/59/569d3c096e542502.png" alt="">
                        <p class="index-icon-item">金融理财</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/a9/ffc620dbda9b9c02.png" alt="">
                        <p class="index-icon-item">保险车险</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/35/2640cab202c41b02.png" alt="">
                        <p class="index-icon-item">全球购</p>
                    </a>
                </div>
                <div class="index-icon">
                    <a href="">
                        <img src="https://imgs.qunarzz.com/piao/fusion/1611/54/ace00878a52d9702.png" alt="">
                        <p class="index-icon-item">度假</p>
                    </a>
                </div>
            </div>
        </swiper-slide>
        <div class="swiper-pagination"  slot="pagination"></div>
        <ul>
            <li></li>
            <li></li>
        </ul>
    </swiper>
</template>

<script>

    import { swiper, swiperSlide } from 'vue-awesome-swiper'

    export default {
        name: 'carrousel',
        data() {
            return {
                notNextTick: true,
                swiperOption: {
                    autoplay: 3000,
                    direction: 'horizontal',
                    autoHeight: true,
                    pagination: '.swiper-pagination',
                    observeParents: true,
                }
            }
        }, 
        components: {
            swiper,
            swiperSlide
        }
    }
</script>

<style scoped>
    .index-icon-swiper {
        overflow: hidden;
        height: 3.7rem;
        padding-top: .1rem;
        background-color: #fff
    }
    .index-icon {
        float: left;
        width: 25%;
        height: 1.3rem;
        padding-top: .3rem;
        text-align: center;
    }
    .index-icon img {
        width: .66rem;
        height: .66rem;
    }
    .index-icon-item {
        overflow: hidden;
        white-space: nowrap;
        text-overflow: ellipsis;
        margin-top: .2rem;
        color: #212121;
        font-size: .28rem;
        text-align: center;
    }
</style>