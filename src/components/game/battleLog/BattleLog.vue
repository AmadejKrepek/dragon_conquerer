<template>
    <div class="container">
        <h4 class="text-center">Battle Logs</h4>
        <ul class="col-md-5 logs">
            <li v-for="logMessage in battleLogMessages" :key="logMessage" class="text-center">
                <span 
                :class="{
                    'warrior' : logMessage.attacker === 'warrior', 'dragon' : logMessage.attacker === 'dragon'
                }">
                <img src="@/assets/gifs/warrior1.gif" alt="warrior" v-if="logMessage.attacker === 'warrior'" class="img-icon">
                <img src="@/assets/gifs/dragon1.gif" alt="dragon" v-else class="img-icon">
                 </span>
                 <span v-if="logMessage.actionType === 'heal'">
                     heals himself for <span class="log-heal">{{ logMessage.actionValue }} of damage</span>
                 </span>
                 <span v-else-if="logMessage.actionType === 'special-attack'">
                     use special attack and deals <span class="log-damage">{{ logMessage.actionValue }} of damage.</span>
                 </span>
            </li>
        </ul>
    </div>
</template>

<script>
export default {
    
}
</script>