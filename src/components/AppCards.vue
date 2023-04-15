<script>
export default {
    name: "AppCards",
    props: {
        thumb: Object
    }
} 
</script>

<template>
    <div class="card">
        <div class="card-image">
            <img :src="thumb.thumb" :alt="thumb.series">
        </div>
        <h4>{{ thumb.series }}</h4>
    </div>
</template>


<style scoped lang="scss">
.card {
    width: calc((100% / 6) - 30px);
    margin: 20px 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
    cursor: pointer;

    & h4 {
        color: white;
    }

    & .card-image {
        width: 100%;
        padding-top: 100%;
        position: relative;

        & img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: top;
            position: absolute;
            top: 0;
        }
    }

}
</style>