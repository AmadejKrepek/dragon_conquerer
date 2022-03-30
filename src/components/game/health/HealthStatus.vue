<template>
    <div class="health">
        <div class="health-bar" :style="healthBarTitle">
            <PercentageStatus :value="healthType" />
        </div>
    </div>
</template>

<script>
import PercentageStatus from './PercentageStatus.vue';

export default {
    components: {
        PercentageStatus
    },
    props: {
        healthBarTitle: String,
        healthType: Number
    }
}
</script>