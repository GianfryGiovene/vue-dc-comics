<template>
    <div class="container">
        <main>
            Content goes here
        </main>
    </div>
</template>

<script>
export default {
    name: 'MainSide',
}
</script>

<style lang="scss" scoped>
.container{
    width: 100%;
    background-color: #1c1c1c;
    flex-grow: 1;
    main{
    max-width: 1200px;
    margin: auto;
    padding: 50px 100px;
    color: #fff;
    font-size: 1.6rem;
    }
}
</style>