<template>
    <header class="container">
      <img src="../assets/img/dc-logo-bg.png" alt="">
        <ul>
            <li v-for="(item,index) in navBar " :key="`navBar-${index}`" :class="{'active': item.isActive}">
                <a  :href="item.href">{{item.name}}</a>
            </li>
            
        </ul>
    </header>      
              
                  
              
              
                  
                
            
                
              
          
      
  
</template>

<script>
export default {
    name: "HeaderComp",
    data(){
        return{
            navBar:[
                {
                    name: "characters",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "comics",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "movies",
                    href: "#",
                    isActive : true
                   
                },
                {
                    name: "tv",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "games",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "collectibles",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "videos",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "fans",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "news",
                    href: "#",
                    isActive : false
                   
                },
                {
                    name: "shop",
                    href: "#",
                    isActive : false
                   
                },
            ]
        }
       
    }
}
</script>

<style lang="scss" scoped>
header{
    width: 100%;
    height: 120px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    
    
}
img{
    
    width: 80px;
    
}
ul{
    display: flex;
    justify-content: center;
    align-items: center;
    list-style: none;
    li{
        margin: 20px;
        text-transform: uppercase;
        &.active{
            border-bottom: 5px solid #1278f9 ;
        }
        a{
            color: black;
            text-decoration: none;
            &:hover{
                color: #1278f9;
            }
        }
        
    }
}

</style>