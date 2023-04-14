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
    box-sizing: border-box;
    margin: 20px 15px;
    display: flex;
    flex-direction: column;
    align-items: center;

    & h4 {
        margin-top: 10px;
        color: white;
    }

    & .card-image {
        width: 100%;
        padding-top: 100%;
        overflow: hidden;
        position: relative;

        & img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            position: absolute;
            top: 0;
            left: 0;
        }
    }

}
</style>