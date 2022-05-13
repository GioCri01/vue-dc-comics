<template>
    <footer>
        <div class="container footer-section">
            <ul>
                <li><h2>dc comics</h2></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
                <li><h3>shop</h3></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>

                
                
            </ul>
            <ul>
                <li><h2>dc</h2></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
                
            </ul>
            <ul>
                <li><h2>sites</h2></li>
                <li><a href="#">Characters</a></li>
                <li><a href="#">Comics</a></li>
                <li><a href="#">Movies</a></li>
                <li><a href="#">TV</a></li>
                <li><a href="#">Games</a></li>
                <li><a href="#">Videos</a></li>
                <li><a href="#">News</a></li>
                
            </ul>

        </div>
        <div class="credits ">
            <div class="container credits-item">
                <button>sign-up now!</button>
                <div class="social">
                    <h3>follow us</h3>
                    <a href="#"><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-youtube.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-pinterest.png" alt=""></a>
                    <a href="#"><img src="../assets/img/footer-periscope.png" alt=""></a>
                    
                </div>
            </div>
        </div>
    </footer>
  
</template>

<script>
export default {
    nane:"FooterComp",

}
</script >


<style lang="scss" scoped>
    footer{
        width: 100%;
        
        background-image: url("../assets/img/footer-bg.jpg");
        background-size:cover ;
    }

    .footer-section{
        display: flex;
        
        padding: 25px 0;
        h2{
            color: white;
            text-transform: uppercase;
            font-size: 20px;
        }
        ul{
            list-style: none;
            li{
                padding: 2px 0;
                a{
                    text-decoration: none;
                    color: gray;
                }
            }
        }
        h3{
            color: white;
            text-transform: uppercase;
            font-size: 20px;
            padding: 8px 0;
        }
    }

    .credits{
        width: 100%;
        height: 100px;
        background-color: #303030;
        display: flex;
        justify-content: center;

    }
    .credits-item{
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    .social{
        display: flex;
        h3{
            padding: 15px;
            text-transform: uppercase;
            color:#0085fb ;
        }
        img{
            padding: 15px;
        }
    }

    button{
        padding: 10px 20px;
        border: 2px solid #0085fb;
        background-color: transparent;
        text-transform: uppercase;
        color: white;
    }

</style>