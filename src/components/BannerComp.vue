<template>
  <div class="banner">
      <div class="container item-container">
          <div class=" item-banner">
          <img src="../assets/img/buy-comics-digital-comics.png" alt="">
          <h2>digital comics</h2>
        </div>
        <div class=" item-banner">
          <img src="../assets/img/buy-comics-merchandise.png" alt="">
          <h2>digital comics</h2>
        </div>
        <div class=" item-banner">
          <img src="../assets/img/buy-comics-shop-locator.png" alt="">
          <h2>digital comics</h2>
        </div>
        <div class=" item-banner">
          <img src="../assets/img/buy-comics-subscriptions.png" alt="">
          <h2>digital comics</h2>
        </div>
        <div class=" item-banner">
          <img src="../assets/img/buy-dc-power-visa.svg" alt="">
          <h2>digital comics</h2>
        </div>
      </div>

      
  </div>
</template>

<script>
export default {
    name:"BannerComp",

}
</script>

<style lang="scss" scoped>
.banner{
    width: 100%;
    height: 200px;
    background-color: #0282f9;
    display: flex;
    justify-content: center;
    align-items: center;
    
}
.item-container{
    display: flex;
    justify-content: space-around;
    align-items: center;

    
    

}
.item-banner{
    display: flex;
    align-items: center;
    h2{
        font-size: 15px;
        text-transform: uppercase;
        margin: 10px;
        color: white;
    }
    
}
img{
    width: 50px;
}

</style>