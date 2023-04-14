<script>
export default {
    name: 'AppFeatures',
}
</script>

<template>
    <div class="container">
        <div class="nav">
            <ul>
                <li>
                    <img src="../assets/img/buy-comics-digital-comics.png" alt="digitalComics">
                    <span>Digital comics</span>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-merchandise.png" alt="merchandaise">
                    <span>DC merchandise</span>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-subscriptions.png" alt="comicsSubscriptions">
                    <span>subscription</span>
                </li>
                <li>
                    <img src="../assets/img/buy-comics-shop-locator.png" alt="shopLocator">
                    <span>Comic shop locator</span>
                </li>
                <li>
                    <img src="../assets/img/buy-dc-power-visa.svg" alt="buyVisa">
                    <span>DC power visa</span>
                </li>
            </ul>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/general.scss" as *;

.container {
    width: 100%;
    height: 150px;
    background-color: lightblue;
    display: flex;
    justify-content: center;
}

.nav {
    display: flex;
    justify-content: center;
}

ul {
    display: flex;
    justify-content: center;
    align-items: center;
}

li {
    display: flex;
    align-items: center;
}

img {
    width: 50px;
}
</style>
