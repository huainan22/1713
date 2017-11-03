<template>
    <div>
    	<index-header />
        <index-swiper />
        <index-homenav />   

    </div>
</template>

<script>
    import header from "./Header.vue";
    import swiper from "./Swiper.vue";
    import homenav from "./Hnav.vue";
    export default {
        components: {
        	"index-header": header,
            "index-swiper": swiper,
            "index-homenav": homenav
        }
    }
</script>


<style scoped>

</style>