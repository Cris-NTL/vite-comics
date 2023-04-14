<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            categories: [
                {
                    name: "Characters",
                    url: "#"
                },
                {
                    name: "Comics",
                    url: "#"
                },
                {
                    name: "Movies",
                    url: "#"
                },
                {
                    name: "TV",
                    url: "#"
                },
                {
                    name: "Games",
                    url: "#"
                },
                {
                    name: "Collectibles",
                    url: "#"
                },
                {
                    name: "Videos",
                    url: "#"
                },
                {
                    name: "Fans",
                    url: "#"
                },
                {
                    name: "News",
                    url: "#"
                },
                {
                    name: "Shop",
                    url: "#"
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
                    <li v-for="name in categories"><a href="#">{{ name.name }}</a></li>
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
</style>
