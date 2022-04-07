<template>
    <main class="container">
        <div class="top">
            <MainCardTop />
        </div>
        <div class="bottom">
            <MainCardBottom />
        </div>
        
    </main>
</template>

<script>
import MainCardTop from './main_components/MainCardTop.vue';
import MainCardBottom from './main_components/MainCardBottom.vue';

export default {
    name: 'MainSide',
    components: {
        MainCardTop,
        MainCardBottom,
    }
   
}
</script>

<style lang="scss" scoped>
@import "./variables";
main{
    width: 100%;
    flex-grow: 1;
    .top{
        width: 100%;
        height: 45%;
        background-color: #1c1c1c;    
        font-size: 1.6rem;
    }
    .bottom{
        width: 100%;
        height: 55%;
        background-color: $blue-DC;
    }
}
</style>