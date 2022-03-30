<template>
    <p class="text-center">{{title}}</p>
    <div class="img-container">
        <img :src="require(`@/assets/gifs/${image}.gif`)" :alt="title">
    </div>
</template>

<script>
export default {
    props: {
        title: String,
        image: String,
    }
}
</script>