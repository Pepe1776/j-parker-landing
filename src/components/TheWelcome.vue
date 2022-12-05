<template>
  <div class="img-cont">
    <transition name="slide-fade">
<img v-show="cue3" src="../assets/jparker_self.png" alt="satoshi shiba inu" class="img satoshi"/>
</transition>
  </div>
  <header>
    <transition name-="slide-fade">
      <div v-show="cue1" class="name-cont">
    <h1 class="name-cap">J</h1><h1 class="name-low">ustin</h1><h1 class="name-cap2">P</h1><h1 class="name-low2">arker</h1>
  </div>
  </transition>
  <transition name="slide-fade">
    <h2 v-show="cue2" class="sub">Software Engineer, Automation Programmer, UI Designer</h2>
  </transition>
  <transition name="slide-fade">
  <button v-show="cue4" class="btn">Browse Work</button>
</transition>
  </header>
</template>

<script setup>
import { ref } from 'vue';

const cue1 = ref(false);
const cue2 = ref(false);
const cue3 = ref(false);
const cue4 = ref(false);

setTimeout(() => {
  cue1.value = true;
}, 500);
setTimeout(() => {
  cue2.value = true;
}, 800);
setTimeout(() => {
  cue3.value = true;
}, 2000);
setTimeout(() => {
  cue4.value = true
}, 3000);
</script>

<style scoped>
.img-cont {
width: 100vw;
height: 100vh;
inset: 0;
}

.img {
  width: 40%;
  height: auto;
  object-fit: contain;
  position: absolute;
  left: 35%;
  bottom: 15%;
  opacity: 0.2;
  border-radius: 40%;
  box-shadow: 0px 0px 15px rgba(59, 58, 58, 0.354);
}
.name-cont {
  width: 100%;
  position: relative;
}
.name-low {
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  font-size: 3rem;
  position: absolute;
  z-index: 2;
  margin-top: -40%;
  left: 1%;
  opacity: 0.3;
}
.name-low2 {
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  font-size: 3rem;
  position: absolute;
  z-index: 2;
  margin-top: -40%;
  left: 15%;
  opacity: 0.3;
}
.name-cap {
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  font-size: 8rem;
  position: absolute;
  z-index: 2;
  margin-top: -45.5%;
  left: -2%;
  opacity: 0.3;
}
.name-cap2 {
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  font-size: 8rem;
  position: absolute;
  z-index: 2;
  margin-top: -45.5%;
  left: 12%;
  opacity: 0.3;
}
.sub {
  position: absolute;
  z-index: 2;
  margin-top: -28%;
  margin-left: -4%;
  opacity: 0.3;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
}
.btn {
  position: absolute;
  z-index: 2;
  margin-top: -22%;
  margin-left: 6.5%;
  opacity: 0.3;
  box-shadow: 0px 0px 15px rgba(59, 58, 58, 0.354);
  color: aliceblue;
  background-color: rgba(59, 58, 58, 0.354);
  padding: 20px;
  font-size: x-large;
  font-family: Impact, Haettenschweiler, 'Arial Narrow Bold', sans-serif;
  border-radius: 10%;
}
.slide-fade-enter-active {
  transition: all 0.6s ease-out;
}
.slide-fade-leave-active {
  transition: all 1s cubic-bezier(1, 0.5, 0.8, 1);
}
.slide-fade-enter-from,
.slide-fade-leave-to {
  transform: translateX(80px);
  transform: translateY(40px);
  opacity: 0;
}
</style>