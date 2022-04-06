<template>
    <footer id="footer">
        <div class="container">
            <div class="flex-wrap">
                <div class="flex-wrap-column">
                <ul>
                    <li>DC COMICS</li>
                    <li>Characters</li>
                    <li>Comics</li>
                    <li>Movies</li>
                    <li>TV</li>
                    <li>Games</li>
                    <li>Videos</li>
                    <li>News</li>
                </ul>
                <ul>
                    <li>SHOP</li>
                    <li>Shop DC</li>
                    <li>Shop DC Collectibles</li>
                </ul>
                <ul>
                    <li>DC</li>
                    <li>Terms of Use</li>
                    <li>Privacy Policy (New)</li>
                    <li>Ad Choices</li>
                    <li>Advertising</li>
                    <li>Jobs</li>
                    <li>Subscriptions</li>
                    <li>Talent Workshops</li>
                    <li>CPSC Certificates</li>
                    <li>Ratings</li>
                    <li>Shop Help</li>
                    <li>Contact Us</li>
                </ul>
                <ul>
                    <li>SITES</li>
                    <li>DC</li>
                    <li>MAD Magazine</li>
                    <li>DC Kids</li>
                    <li>DC Universe</li>
                    <li>DC Power Visa</li>
                </ul>
            </div>
            <img src="../assets/dc-logo-bg.png" alt="dc logo">
            </div>      
        </div>
        <div class="container">
            <div class="flex-wrap">
                <button>SIGN-UP NOW!</button>
                <ul>
                    <li>FOLLOW US</li>
                    <li><img src="../assets/footer-facebook.png" alt=""></li>
                    <li><img src="../assets/footer-twitter.png" alt=""></li>
                    <li><img src="../assets/footer-youtube.png" alt=""></li>
                    <li><img src="../assets/footer-pinterest.png" alt=""></li>
                    <li><img src="../assets/footer-periscope.png" alt=""></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
export default {
    name: 'FooterSide',
    
}

</script>

<style lang="scss" scoped>
$blue-DC:#0282f9;
footer{
    width: 100%;
    .container:first-child{
        width: 100%;
        background-image: url('../assets/footer-bg.jpg');
        
        .flex-wrap{
            display: flex;
            max-width: 1200px;
            margin: auto;
            justify-content: space-between;
            align-items: center;
            height: 400px;
            .flex-wrap-column{
                height: 400px;
                padding: 30px 0; 
                display: flex;
                flex-flow: column wrap;
                align-content: flex-start;
                align-items: flex-start;
                ul{
                    list-style-type: none;
                    padding: 20px;
                    color: #aaa;
                    li:first-child{
                        font-size: 1.2rem;
                        margin-bottom: 20px;
                        color: #fff;
                    }
                
                }
            
            }
            img{
                width: 500px;
                object-fit: cover;
                height: 100%;
            }
        }
    }   

    .container:last-child{
        width: 100%;
        background-color: #303030;
        padding: 20px;
        .flex-wrap{
            padding: 10px;
            max-width: 1200px;
            margin: auto;
            display: flex;
            justify-content: space-between;
            align-items: center;    
        }
        button{
            color: #fff;
            display: inline-block;
            border: 2px solid $blue-DC;
            padding: 8px;
            background: none ;
            cursor: pointer;
            
        }
        ul{
            list-style-type: none;
            display: flex;
            align-items: center;
            gap: 20px;
            li:first-child{
                color: $blue-DC;
                font-weight: 700;
            }
        }
    }
}
</style>