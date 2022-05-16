<template>

  <div class="box">
        <img :src="card.thumb" :alt="card.series">
        <p>{{card.series}}</p>
  </div>

                
    
</template>

<script>
export default {
    name: "CardComp",
    props:{
        card:Object

    }

}
</script>

<style lang="scss" scoped>
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

</style>