<template>
  <div id="app">

    <div class="container-fluid">
      <div class="row no-wrap align-center align-center">
        <div class="col-sm">
          <img class="img-fluid " src="./assets/logos/1.svg" alt="logo">
        </div>
        <div class="col-sm delay-1">
            <img class="img-fluid" src="./assets/logos/2.svg" alt="logo">
            <img class="img-fluid" src="./assets/logos/2.svg" alt="logo">
        </div>
        <div class="col-sm">
            <img class="img-fluid" src="./assets/logos/3.svg" alt="logo">
        </div>
         <div class="col-sm delay-2">
            <img class="img-fluid" src="./assets/logos/4.svg" alt="logo">
        </div>
         <div class="col-sm">
            <img class="img-fluid" src="./assets/logos/5.svg" alt="logo">
        </div>
         <div class="col-sm delay-1">
            <img class="img-fluid" src="./assets/logos/6.svg" alt="logo">
        </div>
         <div class="col-sm">
            <img class="img-fluid" src="./assets/logos/7.svg" alt="logo">
        </div>
         <div class="col-sm delay-2">
            <img class="img-fluid" src="./assets/logos/8.svg" alt="logo">
        </div>
         <div class="col-sm">
            <img class="img-fluid" src="./assets/logos/9.svg" alt="logo">
        </div>
         <div class="col-sm delay-1">
            <img class="img-fluid" src="./assets/logos/10.svg" alt="logo">
        </div>
      </div>
  </div>

    <b-modal id="modal-center" centered>
        <img src="./assets/logos/8.svg" alt="">
        <h4 class="my-1">Titulo</h4>
        <div class="d-flex">
          <div class="d-grid--left">
            <p class="text-left">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium non velit porro error vel magni, autem tenetur ex nemo qui eum officiis praesentium possimus, quas quidem dolores animi placeat. Dolorum!</p>
            <img src="https://via.placeholder.com/150x150" alt="">

          </div>
          <div class="d-grid--right">
            <img src="https://via.placeholder.com/150x150" alt="">
            <p class="text-left">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium non velit porro error vel magni, autem tenetur ex nemo qui eum officiis praesentium possimus, quas quidem dolores animi placeat. Dolorum!</p>

          </div>
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
#app {
  height: 100%;
}

.container-fluid {
  height:inherit;
}

.row {
  height: 100%;
}

.align-center {
  align-content: center;
}

.img-fluid {
	-webkit-animation: vibrate-2 0.75s ease-out 2s infinite both;
	        animation: vibrate-2 0.75s ease-out 2s infinite both;
}

.delay-1 {
  	-webkit-animation: vibrate-2 0.75s ease-out 1s infinite both;
	        animation: vibrate-2 0.75s ease-out 1s infinite both;
}

.delay-2 {
  -webkit-animation: vibrate-2 0.75s ease-out 3s infinite both;
	        animation: vibrate-2 0.75s ease-out 3s infinite both;
}


@-webkit-keyframes vibrate-2 {
  0% {
    -webkit-transform: translate(0);
            transform: translate(0);
  }
  20% {
    -webkit-transform: translate(2px, -2px);
            transform: translate(2px, -2px);
  }
  40% {
    -webkit-transform: translate(2px, 2px);
            transform: translate(2px, 2px);
  }
  60% {
    -webkit-transform: translate(-2px, 2px);
            transform: translate(-2px, 2px);
  }
  80% {
    -webkit-transform: translate(-2px, -2px);
            transform: translate(-2px, -2px);
  }
  100% {
    -webkit-transform: translate(0);
            transform: translate(0);
  }
}
@keyframes vibrate-2 {
  0% {
    -webkit-transform: translate(0);
            transform: translate(0);
  }
  20% {
    -webkit-transform: translate(2px, -2px);
            transform: translate(2px, -2px);
  }
  40% {
    -webkit-transform: translate(2px, 2px);
            transform: translate(2px, 2px);
  }
  60% {
    -webkit-transform: translate(-2px, 2px);
            transform: translate(-2px, 2px);
  }
  80% {
    -webkit-transform: translate(-2px, -2px);
            transform: translate(-2px, -2px);
  }
  100% {
    -webkit-transform: translate(0);
            transform: translate(0);
  }
}


.d-flex > * {
  border:1px solid white;
}

.d-flex  {
  border: 1px solid #f1f1f1;
  .d-grid--right {
    flex: 1;
  }
  .d-grid--left {
    flex:3;
  }
}

.icon {
  margin: 50vh auto;
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #fff;
}
</style>
