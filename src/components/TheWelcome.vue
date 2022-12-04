<template>
  <div class="img-cont">
    <transition name="slide-fade">
<img v-show="cue3" src="../assets/jparker_self.png" alt="satoshi shiba inu" class="img satoshi"/>
</transition>
  </div>
  <header>
    <transition name-="slide-fade">
    <img v-show="cue1" src="../assets/Jparker.png" alt="jparker" class="name">
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

.name {
  position: absolute;
  z-index: 2;
  margin-top: -40%;
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