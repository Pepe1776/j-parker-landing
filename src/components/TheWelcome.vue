<template>
  <div class="img-cont">
    <transition name="slide-fade">
<img v-show="cue4" src="../assets/jparker_self.png" alt="satoshi shiba inu" class="img satoshi"/>
</transition>
  </div>
  <header>
    <transition name-="slide-fade">
      <div class="name-cont">
    <h1 v-show="cue1" class="name-cap">J</h1><h1 v-show="cue2" class="name-low">ustin</h1><h1 v-show="cue3" class="name-cap2">P</h1><h1 v-show="cue4" class="name-low2">arker</h1>
  </div>
  </transition>
  <transition name="slide-fade">
    <h2 v-show="cue4" class="sub">Software Engineer|Automation Programmer|UI Designer</h2>
  </transition>
  <transition name="slide-fade">

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
}, 1000);
setTimeout(() => {
  cue3.value = true;
}, 1500);
setTimeout(() => {
  cue4.value = true
}, 2000);
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
  box-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);
}
.name-cont {
  width: 100%;
  position: relative;
}
.name-low {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 3rem;
  position: absolute;
  z-index: 2;
  margin-top: -30%;
  left: 1.5%;
  color: rgb(25, 25, 25);
  text-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);}
.name-low2 {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 3rem;
  position: absolute;
  z-index: 2;
  margin-top: -30%;
  left: 16.5%;
  color: rgb(25, 25, 25);
  text-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);}
.name-cap {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 25rem;
  font-weight: 100;
  position: absolute;
  z-index: 2;
  margin-top: -55%;
  left: -8%;
  color: rgb(25, 25, 25);
  text-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);
}
.name-cap2 {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 25rem;
  position: absolute;
  z-index: 2;
  margin-top: -55%;
  left: 10%;
  color: rgb(25, 25, 25);
  text-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);}
.sub {
  position: absolute;
  z-index: 2;
  margin-top: -23%;
  margin-left: -10.5%;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  font-size: 1.7rem;
  color: rgb(25, 25, 25);
  text-shadow: -5px 5px 15px rgb(1, 161, 224);}
.btn {
  position: absolute;
  z-index: 2;
  margin-top: -28%;
  margin-left: 4.5%;
  box-shadow: -15px 5px 18px rgba(129, 0, 176, 0.399);
  color: rgba(115, 4, 155, 0.435);
  background-color: rgba(25,25,25);
  padding: 20px;
  font-size: x-large;
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
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