<script>
export default {
    name: 'AppJumbotron',
}
</script>

<template>
    <div class="container">
        <div class="jumbo">
            <img src="../assets/img/jumbotron.jpg" alt="jumbotronImage">
        </div>
    </div>
</template>

<style lang="scss" scoped>
@use "../style/general.scss" as *;

.container {
    width: 100%;
    height: 15rem;
}

.jumbo {
    width: 100%;
    height: 100%;
}

img {
    object-fit: cover;
    object-position: top;
    width: 100%;
    height: 100%;
}
</style>
