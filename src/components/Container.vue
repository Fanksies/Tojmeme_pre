<template>
<div id="container">
    <div class="container-fluid" v-on:click="openMap">
      <div class="row no-wrap align-center align-center">
        <div class="col-sm">
          <img class="animate-logo " src="./assets/logos/1.svg" alt="logo">
        </div>
        <div class="col-sm delay-1">
            <img class="animate-logo" src="./assets/logos/2.svg" alt="logo">
            <img class="animate-logo" src="./assets/logos/2.svg" alt="logo">
        </div>
        <div class="col-sm">
            <img class="animate-logo" src="./assets/logos/3.svg" alt="logo">
        </div>
         <div class="col-sm delay-2">
            <img class="animate-logo" src="./assets/logos/4.svg" alt="logo">
        </div>
         <div class="col-sm">
            <img class="animate-logo" src="./assets/logos/5.svg" alt="logo">
        </div>
         <div class="col-sm delay-1">
            <img class="animate-logo" src="./assets/logos/6.svg" alt="logo">
        </div>
         <div class="col-sm">
            <img class="animate-logo" src="./assets/logos/7.svg" alt="logo">
        </div>
         <div class="col-sm delay-2">
            <img class="animate-logo" src="./assets/logos/8.svg" alt="logo">
        </div>
         <div class="col-sm">
            <img class="animate-logo" src="./assets/logos/9.svg" alt="logo">
        </div>
         <div class="col-sm delay-1">
            <img class="animate-logo" src="./assets/logos/10.svg" alt="logo">
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

<script>
export default {
    name: "Container"
}
</script>