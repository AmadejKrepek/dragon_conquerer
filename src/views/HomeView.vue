<template>
  <div>
    <MainHeader />
    <GameContainer />
  </div>
</template>

<script>
import MainHeader from '../components/header/MainHeader.vue';
import GameContainer from '../components/game/GameContainer.vue';

export default {
  name: 'HomeView',
  components: {
    MainHeader,
    GameContainer
  }
}
</script>
