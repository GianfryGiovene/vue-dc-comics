<template>
    <footer id="footer">
        <div class="container">
            <div class="flex-wrap">
                <div class="flex-wrap-column">
                <ul>
                    <li :key='index' v-for="(element,index) in dcComics">{{ element }}</li>
                    
                </ul>
                <ul>
                    <li :key="index" v-for="(element,index) in shop">{{ element }}</li>
                    
                </ul>
                <ul>
                    <li :key="index" v-for="(element,index) in dc">{{ element }}</li>
                    
                </ul>
                <ul>
                    <li :key="index" v-for="(element,index) in sites">{{ element }}</li>
                    
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
                    <li :key="index" v-for="(element,index) in followUS"><img :src="element.img" :alt="element.description"></li>
                </ul>
            </div>
        </div>
    </footer>
</template>

<script>
import facebook from '../assets/footer-facebook.png';
import twitter from '../assets/footer-twitter.png';
import youTube from '../assets/footer-youtube.png';
import pinterest from '../assets/footer-pinterest.png';
import periscope from '../assets/footer-periscope.png';
export default {
    name: 'FooterSide',
    data: function(){
        return{
            dcComics: ['DC COMICS','Characters','Comics','Movies','TV','Games','Videos','News'],
            shop: ['SHOP','Shop DC','Shop DC Collectibles'],
            dc: ['DC','Terms of Use','Privacy Policy (New)','Ad Choices','Advertising','Jobs','Subscriptions','Talent Workshops','CPSC Certificates','Ratings','Shop Help','Contact Us'],
            sites: ['SITES','DC','MAD Magazine','DC Kids','DC Universe','DC Power Visa'],
            followUS: [
                {
                    img: facebook,
                    description:'facebook'
                },
                {
                    img: twitter,
                    description:'twitter'
                },
                {
                    img: youTube,
                    description: 'youtube'
                },
                {
                    img: pinterest,
                    description: 'pinterest'
                },
                {
                    img: periscope,
                    description: 'periscope'
                }],
        }
    }
    
}

</script>

<style lang="scss" scoped>
@import "./variables";
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