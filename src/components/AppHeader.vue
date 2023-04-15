<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            categories: [
                {
                    name: "Characters",
                    url: "#",
                    current: false
                },
                {
                    name: "Comics",
                    url: "#",
                    current: true
                },
                {
                    name: "Movies",
                    url: "#",
                    current: false
                },
                {
                    name: "TV",
                    url: "#",
                    current: false
                },
                {
                    name: "Games",
                    url: "#",
                    current: false
                },
                {
                    name: "Collectibles",
                    url: "#",
                    current: false
                },
                {
                    name: "Videos",
                    url: "#",
                    current: false
                },
                {
                    name: "Fans",
                    url: "#",
                    current: false
                },
                {
                    name: "News",
                    url: "#",
                    current: false
                },
                {
                    name: "Shop",
                    url: "#",
                    current: false
                },
            ],
        };
    },
};
</script>

<template>
    <div class="container">
        <div class="wrap">
            <div class="logo">
                <img src="../assets/img/dc-logo.png" alt="logoImage">
            </div>
            <nav>
                <ul>
                    <li v-for="(link, index) in categories" :key="index">
                        <a :href="link.url" :class="{ active: link.current }">
                            {{ link.name }}
                        </a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/general.scss" as *;
@use "../style/app-header" as *;
</style>
