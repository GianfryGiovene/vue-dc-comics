<template>
    <header>
        <img src="../assets/dc-logo.png" alt="dc-logo">
        <ul>
            <li :key='index' v-for='(element,index) in navArray'>{{ element }}</li> 
        </ul>
    </header>
</template>

<script>

export default {
    name: 'HeaderSide',
    data: function(){
        return{
            navArray: ['CHARACTERS','COMICS','MOVIES','TV','GAMES','COLLECTIBLES','VIDEOS','FANS','NEWS','SHOP']
        }
    }
}

</script>

<style lang="scss" scoped>

@import "./variables";
header{
    width: 1200px;
    margin: auto;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: space-between;  
    img{
        width: 80px;
    }
    ul{
        height: 100%;
        align-items:center;
        list-style-type: none;
        display: flex;
        gap: 10px;
        li{

            &:hover{
                color: $blue-DC ;
                border-bottom: 2px solid $blue-DC;
            }
        }
    }
}
</style>

