<template>
<div id="app" class="bg-secondary ">

    <nav class="navbar bg-light ml-auto">
        <div class="col-md-4">
            <h3 id='nav'>Event Handling</h3>
        </div>

    </nav>
    <div class="row mb-5 mt-3">
        <div class="col-md-4"></div>
        <div class="col-md-4">
            <div class="card ">
                <div class="mt-2 mr-auto ml-1 mb-2">
                    <img src="./assets/4.jpg" alt="" class="img-fluid rounded-circle logo">
                    Pho_stang
                </div>
                <div class="">
                    <img class="img-fluid  " src="./assets/1.jpg">
                </div>

                <div class="card-body">
                    <CsButton></CsButton>
                </div>
            </div>
        </div>
        <div class="col-md-4"></div>

    </div>
    <div class="row mb-5">
        <div class="col-md-4"></div>
        <div class="col-md-4">
            <div class="card ">
                <div class="mt-2 mr-auto ml-1 mb-2">
                    <img src="./assets/4.jpg" alt="" class="img-fluid rounded-circle logo">
                    Pho_stang
                </div>
                <div class="">
                    <img class="img-fluid  " src="./assets/2.jpg">
                </div>

                <div class="card-body">
                    <CsButton></CsButton>
                </div>
            </div>
        </div>
        <div class="col-md-4"></div>

    </div>
    <div class="row mb-5">
        <div class="col-md-4"></div>
        <div class="col-md-4">
            <div class="card ">
                <div class="mt-2 mr-auto ml-1 mb-2">
                    <img src="./assets/4.jpg" alt="" class="img-fluid rounded-circle logo">
                    Pho_stang
                </div>
                <div class="">
                    <img class="img-fluid  " src="./assets/3.jpg">
                </div>

                <div class="card-body">
                    <CsButton></CsButton>
                </div>
            </div>
        </div>
        <div class="col-md-4"></div>

    </div>

    <footer class="mt-5 bg-white ">
        <div class="row mt-3">
            <div class="col-md-4">
                <h3>ABOUT</h3>
                <p class=" box">This website was created as part of the CS313:Web Application Development subject.</p>
            </div>
            <div class="col-md-4">
                <h3>
                    POWERED BY
                </h3>
                <a href="https://vuejs.org/" target="_blank">
                    <img src="./assets/logo.png" class="logofooter">
                </a>
                <a href="https://code.visualstudio.com/" target="_blank">
                    <img src="./assets/Vs_icon.svg" class="logofooter">
                </a>

            </div>
            <div class="col-md-4 ">
                <h3>
                    FOLLOW US
                </h3>
                <div>
                    <a href="https://www.facebook.com/" target="_blank"><img src="./assets/fb.png" alt="" class="icon"></a>
                    <a href="https://www.instragram.com" target="_blank"><img src="./assets/ig.png" alt="" class="icon"></a>
                    <a href="https://www.twitter.com" target="_blank"><img src="./assets/twitter.png" alt="" class="icon"></a>
                    
                </div>

            </div>
            
        </div>

    </footer>
</div>
</template>

<script>
import CsButton from './components/CsButton.vue'
export default {
    name: 'App',
    components: {
        CsButton
    },

    data: function () {
        return {
            total: 0,
        }

    },

    methods: {

        //3.คำนวณผลรวมทั้งหมดที่ส่งออกมาจากemit
        //แล้วนำมาเก็บผลรวมไว้ที่  this.total
        sum(counter) {
            this.total += counter
        },
    },

}
</script>

<style>
#app {
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: black;

}

h3#nav {
    text-align: left;
    font-family: 'Open Sans Condensed', sans-serif;
}

.logo {
    width: 30px;
}

.logofooter {
    width: 80px;
    margin: 10px;
}

footer {
    font-family: 'Open Sans Condensed', sans-serif;
}

p.box {
    width: 150px;
    white-space:initial;
    white-space:normal;
    text-align: center;
    word-wrap: break-word;
    margin: auto;
}
.icon{
    width: 35px;
    margin: 5px;

}
</style>
