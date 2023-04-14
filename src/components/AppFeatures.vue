<script>
export default {
    name: 'AppFeatures',

    data() {
        return {
            features: [
                {
                    img: 'buy-comics-digital-comics.png',
                    description: 'Digital comics',
                },
                {
                    img: 'buy-comics-merchandise.png',
                    description: 'DC merchandise',
                },
                {
                    img: 'buy-comics-subscriptions.png',
                    description: 'Subscription',
                },
                {
                    img: 'buy-comics-shop-locator.png',
                    description: 'Comic shop locator',
                },
                {
                    img: 'buy-dc-power-visa.svg',
                    description: 'DC power visa',
                }
            ]
        }
    },

    methods: {
        getImagePath(img) {
            return new URL(`../assets/img/${img}`, import.meta.url).href;
        }
    }
}
</script>

<template>
    <div class="container">
        <div class="nav">
            <ul>
                <li v-for="(feature, index) in features" :key="index">
                    <img :src="getImagePath(feature.img)" :alt="feature.description">
                    <span>{{ feature.description }}</span>
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
    background-color: #0282f9;
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
    color: white;
    margin-right: 40px;
}

img {
    width: 50px;
    margin-right: 10px;
}
</style>
