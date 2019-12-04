<template>
    <div id="app">

        <div class="container-fluid" v-on:click="openMap">
            <h1 class="display-3 main-title" v-bind:class="{'fade-in': isMapOpen }"> Toj̓ ̓ me me </h1>
            <div class="d-grid">
                <div class="diamond first-diamond" v-bind:class="{'fade-in': isMapOpen }" v-b-modal.modal-1></div>
                <div class=""></div>
                <div class=""></div>
                <div class=""></div>
                <div class="diamond sixth-diamond" v-bind:class="{'fade-in': isMapOpen }"></div>
                <div class=""></div>
                <div class="diamond third-diamond" v-bind:class="{'fade-in': isMapOpen }"></div>
                <div class=""></div>
                <div class="diamond fifth-diamond" v-bind:class="{'fade-in': isMapOpen }"></div>
                <div class=""></div>
                <div class="diamond second-diamond" v-bind:class="{'fade-in': isMapOpen }"></div>
                <div class=""></div>
                <div class="diamond fourth-diamond" v-bind:class="{'fade-in': isMapOpen }"></div>
                <div class=""></div>
                <div class="diamond seventh-diamond" v-bind:class="{'fade-in': isMapOpen }"></div>
            </div>
            <div class="row no-wrap align-center align-center transition">
                <div class="col-sm" v-bind:class="{'img-1': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo" src="./assets/logos/1.svg" alt="logo" ref="test">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-2': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo delay-2" src="./assets/logos/2.svg" alt="logo">
                        <img class="img-fluid animate-logo delay-2" src="./assets/logos/2.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-3': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo" src="./assets/logos/3.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-4': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo delay-1" src="./assets/logos/4.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-5': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo" src="./assets/logos/5.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-6': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo delay-2" src="./assets/logos/6.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-7': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo" src="./assets/logos/7.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-8': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo delay-1" src="./assets/logos/8.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-9': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo" src="./assets/logos/9.svg" alt="logo">
                    </div>
                </div>
                <div class="col-sm" v-bind:class="{'img-10': isMapOpen }">
                    <div>
                        <img class="img-fluid animate-logo delay-2" src="./assets/logos/10.svg" alt="logo">
                    </div>
                </div>
            </div>
        </div>

        <b-modal id="modal-1" centered>
            <img class="modal-logo" src="./assets/logos/8.svg" alt="">
            <h3 class="my-1 mb-4 font-weight-bold text-uppercase">Titulo</h3>
            <div class="d-flex">
                <div class="d-grid--left">
                    <p class="text-left p-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium non velit
                        porro error vel magni, autem tenetur ex nemo qui eum officiis praesentium possimus, quas quidem
                        dolores animi placeat. Dolorum!</p>

                </div>
                <div class="d-grid--right">
                    <img src="https://via.placeholder.com/150x150" alt="">
                    <p class="text-left p-2">Lorem ipsum dolor sit amet consectetur adipisicing elit. Laudantium non velit
                        porro error vel magni, autem tenetur ex nemo qui eum officiis praesentium possimus, quas quidem
                        dolores animi placeat. Dolorum!</p>

                </div>
            </div>
        </b-modal>
    </div>
</template>

<script lang="js">
    import {Component, Vue} from 'vue-property-decorator';
    import Icon from './components/Mask.vue';

    @Component({
        components: {
            Icon
        },
        data() {
            return {
                isMapOpen: false,
            }
        },
        methods: {
            openMap() {
                this.isMapOpen = true;
            },
        }
    })
    export default class App extends Vue {

    }

</script>

<style lang="scss">
    #app {
        height: 100%;
    }

    .container-fluid {
        height: inherit;
    }

    .row {
        height: 100%;
    }

    .align-center {
        align-content: center;
    }

    .animate-logo {
        -webkit-animation: vibrate-2 900ms ease-out 2s infinite both;
        animation: vibrate-2 900ms ease-out 2s infinite both;
    }

    .transition > * {
        transition: all 1200ms ease-out;
    }

    .delay-1 {
        -webkit-animation: vibrate-2 850ms ease-in infinite both;
        animation: vibrate-2 850ms ease-in infinite both;
    }

    .delay-2 {
        -webkit-animation: vibrate-2 800ms ease-in-out infinite both;
        animation: vibrate-2 800ms ease-in-out infinite both;
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
        border: 1px solid white;
    }

    .d-flex {
        border: 1px solid #f1f1f1;

        .d-grid--right {
            flex: 1;
        }

        .d-grid--left {
            flex: 3;
        }
    }

    .icon {
        margin: 50vh auto;
    }

    .fish-offset {
        transform: translateY(1em) !important;
    }

    #app {
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #fff;
    }

    .col-sm {
        display: inline-block;
    }

    .img-1 {
        opacity: .2;
    }

    .img-2 {
        transform: translateY(28em);
        opacity: .2;
    }

    .img-3 {
        transform: translateY(20em);
        opacity: .2;
    }

    .img-4 {
        transform: translateY(12em);
        opacity: .2;
    }

    .img-5 {
        transform: translateY(26em);
        opacity: .2;
    }

    .img-6 {
        opacity: .2;
    }

    .img-7 {
        transform: translateY(18em);
        opacity: .2;
    }

    .img-8 {
        transform: translateY(7em);
        opacity: .2;
    }

    .img-9 {
        transform: translateY(-17em);
        opacity: .2;
    }

    .img-10 {
        opacity: .2;
    }

    .main-title {
        position: absolute;
        margin: 0 auto;
        margin-top: 0px;
        text-align: center;
        width: 100%;
        margin-top: 2em;
        opacity: 0;
        transition: all 4200ms ease-out;
        font-family: 'Kavivanar', cursive;
    }

    .fade-in {
        opacity: 1 !important;
    }

    .d-grid {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr 1fr;
        height: 100%;
        position: absolute;
        opacity: .8;
        width: 100%;
    }

    .diamond {
        opacity: 0;
        width: 2em;
        height: 2em;
        cursor: pointer;
        transform: rotate(45deg);
        border-radius: 10px;
        background: #ffffff6e;
        transition: all 3800ms ease-in;

        &:hover {
            transition: none;
            background: white;
        }
    }

    .first-diamond {
        align-self: end;
        justify-self: flex-end;
    }

    .second-diamond {
        justify-self: end;
    }

    .third-diamond {
        justify-self: end;
        align-self: center;
    }

    .fourth-diamond {
        justify-self: center;
        align-self: center;
    }

    .fifth-diamond {
        align-self: center;
    }

    .sixth-diamond {
        align-self: end;
    }

    .seventh-diamond {

    }

    .modal-content {
        background: #ddd !important;
    }

    .modal-logo {
        vertical-align: middle;
        border-style: none;
        background: #484848;
        height: 120px;
        width: 120px;
        border-radius: 50%;
        padding: 10px;
    }


</style>
