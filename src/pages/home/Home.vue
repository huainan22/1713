<template>
    <div>
        <index-header />
        <index-swiper />
        <index-swiper :swiperInfo="swiperInfo"/>
        <index-icon-swiper />
        <index-address />
        <index-hotlist />
        <index-weekendList />
    </div>
</template>


<script>
    import header from "./component/Header.vue";
    import swiper from "./component/Swiper.vue";
    import indexIconSwiper from "./component/IndexIconSwiper";
    import address from "./component/Address.vue";
    import weekendList from "./component/Weekendlist.vue";
    import hotlist from "./component/HotList.vue";
    import axios from 'axios';

    export default {
        components: {
            "index-header": header,
            "index-swiper": swiper,
            "index-icon-swiper": indexIconSwiper,
            "index-address": address,
            "index-weekendList": weekendList,
            "index-hotlist": hotlist
        },
        data() {
            return {
                swiperInfo: [],
            }
        },
        mounted() {
            this.getHomeData();
        },
        methods: {

            getHomeData() {
                axios.get('../../../static/index.json?city=北京')
                  .then(this.handleGetDataSucc.bind(this))
                  .catch(this.handleGetDataError.bind(this));
            },

            handleGetDataSucc(response) {
                const res = response.data
                const data = res.data;

                this.swiperInfo = data.swiperInfo;
            },

            handleGetDataError(err) {
                console.log(123)
            }
        }

    }

</script>


<style scoped>

</style>
