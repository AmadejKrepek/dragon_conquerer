<template>
    <button :class="`control-icon ${classAction}`" @click="methodName" :disabled="(numOfSpecialAttack === 0 && specialAttack) || (numOfHeal === 0 && isHealAction)">
        <img :src="require(`@/assets/img/${image}`)" :alt="classAction">
        <span class="num-of-attempt" v-if="isHealAction">{{ numOfHeal }}</span>
    </button>
</template>

<script>
export default {
    data() {
        return {
            numOfHeal: 0
        };
    },
    props: {
        image: String,
        methodName: String,
        classAction: String,
        specialAttack: Boolean,
        isHealAction: Boolean
    },
    methods: {
        numOfSpecialAttack() {

        },
    }
}
</script>