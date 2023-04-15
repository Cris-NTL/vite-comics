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
@use "../style/app-cards" as *;
</style>