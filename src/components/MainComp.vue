<template>
  <main >
      <div class=" container-fluid jumbotron">
          
      </div>
      
      <div class="container position-relative">
          <span>current series</span>
          <div class="box-container">
              <div class="box" v-for="(item,index) in DcComics" :key="`item-${index}`">
              <img :src="item.thumb" :alt="item.series">
              <p>{{item.series}}</p>
          </div>
          </div>
          
          
          
      </div>
      <div class="container buttom-container">
          <button>load more</button>
      </div>
      
  </main>
</template>

<script>
import DcComics from "../assets/data/DcComics"

export default {
    name:"MainComp",
    data(){
       return{
           DcComics
       }
    },
    

}
</script>

<style lang="scss" scoped>
    main{
        width: 100%;
        
        background-color: black;
        color: white;
    }
    span{
            position: absolute;
            top: 0;
            left: 0;
            margin-top:-20px ;
            display: inline-block;
            width: 300px;
            height: 50px;
            background-color: #0282f9;
            text-transform: uppercase;
            font-size: 25px;
            text-align: center;
            line-height: 50px;
        }
    .jumbotron{
        position: relative;
        background-image: url("../assets/img/jumbotron.jpg");
        width: 100%;
        height: 300px;

        
        
        
        
        
    }
    .box-container{
        padding: 50px 0;
        display: flex;
        
        flex-wrap: wrap;
    }
    .box{
        margin: 20px 10px;
        
        width: calc(100% /7);

        &:hover{
            transform: scale(1.2);
            cursor: pointer;
        }
        
        
        img{
            width: 100%;
        }
        p{
            margin: 10px;
            color: gray;
        }
        
        
    }
    .buttom-container{
        display: flex;
        justify-content: center;

        button{
        text-align: center;
        padding: 8px 30px;
        background-color:#0282f9 ;
        border: none;
        margin: 15px;
        text-transform: uppercase;
        color: white;
    }

    }

    
    

</style>