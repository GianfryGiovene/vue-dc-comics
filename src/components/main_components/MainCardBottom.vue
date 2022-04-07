<template>
    <div>
        <div :key="index" v-for="(card,index) in cards" class="card">
            <img :src="card.src" :alt="card.name">
            <span>{{ card.name }}</span>
        </div>
    </div>
</template>

<script>

import digital from '@/assets/buy-comics-digital-comics.png';
import merchandise from '@/assets/buy-comics-merchandise.png';
import subscription from '@/assets/buy-comics-subscriptions.png';
import locator from '@/assets/buy-comics-shop-locator.png';
import powerVisa from '@/assets/buy-dc-power-visa.svg';

export default {
    name: 'MainCardBottom',
    data: function(){
        return {
            
            cards: [
                {
                    src: digital,
                    name: 'DIGITAL COMICS'
                },
                {
                    src: merchandise,
                    name: 'DC MERCHANDISE'
                },
                {
                    src: subscription,
                    name: 'SUBSCRIPTION'
                },
                {
                    src: locator,
                    name: 'COMIC SHOP LOCATOR'
                },
                {
                    src: powerVisa,
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