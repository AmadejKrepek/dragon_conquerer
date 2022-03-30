<template>
    <div id="game">
        <div class="container">
            <div class="row">
                <div class="col">
                    <HealthStatus healthBarTitle="warriorHealthBar" :healthType="warriorHealth" />
                    <VisualFigure title="Warrior" image="warrior1" />
                </div>
                <div class="col">
                    <HealthStatus healthBarTitle="dragonHealthBar" :healthType="dragonHealth" />
                    <VisualFigure title="Dragon" image="dragon1" />
                </div>
            </div>
            <div class="row">
                <div class="col controls">
                    <AllControls />
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import HealthStatus from './health/HealthStatus.vue';
import VisualFigure from './figure/VisualFigure.vue';
import AllControls from './controls/ActionControls.vue';

export default {
    components: {   
        HealthStatus,
        VisualFigure,
        AllControls
    }
}
</script>