<template>
    <button :class="`control-icon ${classAction}`" @click="methodName">
        <img :src="require(`@/assets/img/${image}`)" :alt="classAction">
    </button>
</template>

<script>
export default {
    props: {
        image: String,
        methodName: String,
        classAction: String
    }
}
</script>