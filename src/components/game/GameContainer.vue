<template>
    <div id="game">
        <div class="container">
            <div class="row">
                <div class="col">
                    <HealthStatus healthBarTitle="warriorHealthBar" :healthType="5" />
                    <VisualFigure title="Warrior" image="warrior1" />
                </div>
                <div class="col">
                    <HealthStatus healthBarTitle="dragonHealthBar" :healthType="10" />
                    <VisualFigure title="Dragon" image="dragon1" />
                </div>
            </div>
            <div class="row">
                <div class="col controls">
                    <AllControls />
                </div>
            </div>
            <div class="row mt-5">
                <BattleLog />
            </div>
            
            <FinalTime />

        </div>
    </div>
</template>

<script>
import HealthStatus from './health/HealthStatus.vue';
import VisualFigure from './figure/VisualFigure.vue';
import AllControls from './controls/AllControls.vue';
import BattleLog from './battleLog/BattleLog.vue';
import FinalTime from './finalTime/FinalTime.vue';

export default {
    components: {   
        HealthStatus,
        VisualFigure,
        AllControls,
        BattleLog,
        FinalTime
    }
}
</script>