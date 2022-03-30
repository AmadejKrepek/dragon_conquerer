<template>
    <ActionControls classAction="attack" image="attack_icon.svg" methodName="attackDragon" />
    <ActionControls classAction="" image="special_attack.svg" methodName="specialAttack" :specialAttack="true" />
    <ActionControls classAction="" image="heal_icon.png" methodName="heal" :isHealAction="true" />
    <ActionControls classAction="" image="surrender_icon.png" methodName="forfeit" />
</template>

<script>
import ActionControls from './ActionControls.vue';

export default {
    components: {
        ActionControls
    }
}
</script>