<template>
  <div id="app">
    <Icon class="icon" v-b-modal.modal-center/>
    <b-modal id="modal-center" centered>
      <p class="mb-0">This is a logo</p>
      <div class="bg-dark">
        <object type="image/svg+xml" data="/assets/logos/Group.svg" class="logo"></object>
      </div>
    </b-modal>
  </div>
</template>

<script lang="ts">
import { Component, Vue } from 'vue-property-decorator';
import Icon from './components/Mask.vue';

@Component({
  components: {
    Icon
  },
})
export default class App extends Vue {}
</script>

<style lang="scss">
.icon {
  margin: 50vh auto;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
</style>
