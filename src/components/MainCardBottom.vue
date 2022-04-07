<template>
    <div>
        <div :key="index" v-for="(card,index) in cards" class="card">
            <img src="../assets/buy-comics-digital-comics.png" alt="">
            <span>{{ card.name }}</span>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MainCardBottom',
    data: function(){
        return {
            
            cards: [
                {
                    src: '../assets/buy-comics-digital-comics.png',
                    name: 'DIGITAL COMICS'
                },
                {
                    src: '../assets/buy-comics-merchandise.png',
                    name: 'DC MERCHANDISE'
                },
                {
                    src: '../assets/buy-comics-subscription.png',
                    name: 'SUBSCRIPTION'
                },
                {
                    src: '../assets/buy-comics-shop-locator.png',
                    name: 'COMIC CHOP LOCATOR'
                },
                {
                    src: '../assets/buy-dc-power-visa.png',
                    name: 'DP POWER VISA'
                }
            ],
            

        }
    }

}
</script>

<style lang="scss" scoped>

div{
    color: #fff;
    max-width: 1200px;
    margin: auto;
    display: flex;
    height: 100%;
    align-items: center;
    gap: 20px;
    .card{
        display: flex;
        gap: 10px;
        
    }
}

</style>