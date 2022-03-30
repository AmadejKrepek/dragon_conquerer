<template>
    <div class="overlap" v-if="winner">
        <div class="winner">
            <div class="text-center">
                <h3>
                    Game Over!
                </h3>
                <h4 v-if="winner === 'dragon'">You Lose!</h4>
                <h4 v-if="winner === 'warrior'">You Win!</h4>
                <h4 v-else-if="winner === 'draw'">It's a Draw!</h4>
                <button class="btn start-btn mt 4" @click="startFight">Battle Again</button>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        winner: String
    }
}
</script>