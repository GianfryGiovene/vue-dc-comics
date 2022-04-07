<template>
    <div>   
        <img :src="thumb" :alt="series" />
        <span>{{ series }}</span> 
    </div>
</template>

<script>

export default {
    name: 'MainCardTop',
    props:{
        thumb: String,
        price: String,
        series: String,
        type: String,
    }
}


</script>

<style lang="scss" scoped>

div{
    position: relative;
    vertical-align: middle;
    display: flex;
    flex-direction: column;
    color: #fff;
    width: calc(100% / 6 - 1rem);
    margin: auto;
    align-items: center;
    margin-bottom: 30px;
    img{
        width: 100%;
    }
    span{
        text-align: center;
        display: inline-block;
        width: 100%;
        padding: 20px 0;
        position: absolute;
        bottom: 0px;
        background-color: #1c1c1c;
    }
}
</style>