<template>
    <main>
        <div class="jumbotron">
            
        </div>
        <div class="top">
            <span>CURRENT SERIES</span>
            <div class="container">
                <MainTopCard :key="index" v-for="(comic,index) in comics" :thumb="comic.thumb" :price="comic.price" :series="comic.series" :type="comic.type" />      
            </div>
            <button>LOAD MORE</button>
        </div>
        <div class="bottom">
            <MainBottom />
        </div>
        
    </main>
</template>

<script>
import MainTopCard from './main_components/MainTopCard.vue';
import MainBottom from './main_components/MainBottom.vue';
import dcComics from '@/assets/dc-comics.json';

export default {
    name: 'MainSide',
    components: {
        MainTopCard,
        MainBottom,
    },
    data: function(){
        return{
            comics:dcComics,
        }
    }
   
}
</script>

<style lang="scss" scoped>
@import "./variables";
main{
    width: 100%;
    flex-grow: 1;
    .jumbotron{
        background-image: url('@/assets/jumbotron.jpg');
        height: 350px;
        background-size: cover;
    }
    .top{
        width: 100%; 
        background-color: #1c1c1c;   
        display: flex;
        flex-direction: column; 
        justify-content: center;
        align-items: center;
        position: relative;
        span{
            color: #fff;
            left: 350px;
            top: -30px;
            position: absolute;
            font-size: 2rem;
            display: inline-block;
            align-self: flex-start;
            background-color: $blue-DC;
            padding: 10px 20px;
        }
        .container{
            height: 100%;
            max-width: 1200px;
            margin: auto;
            padding: 40px;
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            align-content: center;
        }
        button{
            background-color: $blue-DC;
            color: #fff;
            padding: 10px 35px;
            display: inline-block;
            text-align: center;
            margin-bottom: 40px;
            border: none;
            cursor: pointer;
        }
    }
    .bottom{
        width: 100%;
        padding: 40px 0;
        background-color: $blue-DC;
    }
}
</style>