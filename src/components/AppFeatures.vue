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
@use "../style/app-features.scss" as *;


</style>
