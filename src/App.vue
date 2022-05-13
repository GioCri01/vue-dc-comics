<template>
  <div >
   <HeaderComp/>
   <MainComp/>
   <BannerComp/>
   <FooterComp/>
  </div>
</template>

<script>
import HeaderComp from "./components/HeaderComp.vue"
import MainComp from "./components/MainComp.vue"
import BannerComp from "./components/BannerComp.vue"
import FooterComp from "./components/FooterComp.vue"


export default {
  name :"app",
  components:{
    HeaderComp,
    MainComp,
    BannerComp,
    FooterComp
}
  
}
</script>

<style lang="scss">

</style>
