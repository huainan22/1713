<template>
  <div>
  	 <index-header />
   
  </div>
</template>

<script>
import header from "./Header.vue";
export default {
  name: 'Home',
  data () {
    return {
      
    }
  },
  components: {
  	"index-header": header
  }
}
</script>


<style scoped>

</style>