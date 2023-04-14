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

.container {
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: center;
}

.wrap {
    width: 80%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

img {
    width: 40px;
}

nav {
    width: 70%;

}

ul {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
}

li {
    border-bottom: 6px solid transparent;

    &:hover,
    &.active {
        border-bottom: 6px solid #0282f9;
    }
}
</style>
