<template>
  <div >
   <HeaderComp/>
   <MainComp/>
   <BannerComp/>
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue"
import MainComp from "./components/MainComp.vue"
import BannerComp from "./components/BannerComp.vue"


export default {
  name :"app",
  components:{
    HeaderComp,
    MainComp,
    BannerComp
}
  
}
</script>

<style lang="scss">

</style>
