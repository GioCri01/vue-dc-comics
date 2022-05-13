<template>
  <div class="banner">
      <div class="container item-container">
          <div v-for="(item,index) in oggBanner" :key="`oggBanner-${index}`" class=" item-banner">
          <img :src="item.image" alt="">
          <h2>{{item.name}}</h2>
        </div>
        
      </div>

      
  </div>
</template>

<script>
 import imageUno from "../assets/img/buy-comics-digital-comics.png";
 import imageDue from "../assets/img/buy-comics-merchandise.png";
 import imageTre from "../assets/img/buy-comics-shop-locator.png";
 import imageQuattro from "../assets/img/buy-comics-subscriptions.png";
 import imageCinque from "../assets/img/buy-dc-power-visa.svg";
 
export default {
    name:"BannerComp",
    data(){
        return{
             oggBanner:[
            {
                name:"digital comics",
                image: imageUno
            },
            {
                name:"dc merchandise",
                image: imageDue
            },
            {
                name:"subscription",
                image: imageTre
            },
            {
                name:"comic shop locator",
                image: imageQuattro
            },
            {
                name:"dc power visa",
                image: imageCinque
            },
        ]
        }
       
    }

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