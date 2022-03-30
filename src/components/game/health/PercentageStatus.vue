<template>
    <span class="hp-percent">
        {{ value }} %
    </span>
</template>

<script>
export default {
    props: {
        value: Number
    }
}
</script>