<template>
  <div class="img-cont">
    <transition name="slide-fade">
<img v-show="cue2" src="../assets/jparker_self.png" alt="satoshi shiba inu" class="img satoshi"/>
</transition>
  </div>
  <header>
    <transition name-="slide-fade">
      <div class="name-cont">
<img v-show="cue1" class="name-cap" src="../assets/jp_white.png" alt="JParker">
      </div>
  </transition>
  <transition name="slide-fade">
    <h2 v-show="cue3" class="sub">Software Engineer | Automation Programmer | UI Designer</h2>
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
  left: 25%;
  bottom: 12%;
  opacity: 0.2;
  border-radius: 40%;
  box-shadow: -5px 5px 18px rgb(1, 183, 255);
}
.name-cont {
  width: 100%;
  position: relative;
}

.name-cap {
  width: 45%;
  position: absolute;
  z-index: 2;
  margin-top: -42%;
  left: -20%;
  opacity: 0.6;
}
.sub {
  position: absolute;
  z-index: 2;
  margin-top: -23%;
  margin-left: -24%;
  font-family: 'raleway', serif;
  font-size: 1.8rem;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);}
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