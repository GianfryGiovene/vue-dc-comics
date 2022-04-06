<template>
    <header>
        <img src="../assets/dc-logo.png" alt="dc-logo">
        <ul>
            <li>CHARACTERS</li>
            <li>COMICS</li>
            <li>MOVIES</li>
            <li>TV</li>
            <li>GAMES</li>
            <li>COLLECTIBLES</li>
            <li>VIDEOS</li>
            <li>FANS</li>
            <li>NEWS</li>
            <li>SHOP</li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'HeaderSide',
}


</script>

<style lang="scss"scoped>
$blue-DC:#0282f9;
header{
    width: 100%;
    height: 50px;
    display: flex;
    align-items: center;
    justify-content: space-evenly;
    ul{
        list-style-type: none;
        display: flex;
        li{
            padding: 5px;
            &:hover{
                color: $blue-DC ;
                border-bottom: 2px solid $blue-DC;
            }
        }
    }
}
</style>

