<template>
  <div class="img-cont">
    <transition name="slide-fade">
<img v-show="cue2" src="../assets/DALL·E 2022-12-11 19.55.55 -  Black Shiba Inu as king of space in a paiting.png" alt="satoshi shiba inu" class="img satoshi"/>
</transition>
  </div>
  <img class="img2" src="../assets/vecteezy_abstract-white-and-grey-background-texture_6033460.png" />
  <header>
    <transition name-="slide-fade">
      <div class="name-cont">
<img v-show="cue1" class="name-cap" src="../assets/jp_white.png" alt="JParker">
      </div>
  </transition>
  <div class="sub-cont">
  <transition name="slide-fade">
    <h2 v-show="cue3" class="sub">Software Engineer | Automation Programmer | UI Designer</h2>
  </transition>
</div>
  <transition name="slide-fade">
    <img v-show="cue4" src="../assets/shiba1.jpg" alt="satoshi shiba inu" class="img satoshi"/>
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


</script>

<style scoped>
.img-cont {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100vw;
  height: auto;
  margin-top: 5%;
}

.img {
  width: 40vw;
  height: auto;
  object-fit: contain;
  display: flex;
  align-items: center;
  justify-content: center;
  opacity: 0.2;
  border-radius: 40%;
  box-shadow: -5px 5px 18px rgb(1, 183, 255);
  
}
.name-cont {
  position: relative;
  display: flex;
  justify-content: center;
  align-items: center;
}

.name-cap {
  justify-content: center;
  align-items: center;
  width: 45vw;
  position: absolute;
  z-index: 2;
  margin-top: -15%;
  left: 31%;
  opacity: 0.6;
}

.sub-cont {
  display: flex;
  justify-content: center;
  align-items: center;
}
.sub {
  z-index: 2;
  display: flex;
  justify-content: center;
  align-items: center;
  font-family: 'raleway', serif;
  font-size: 1.8vw;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  margin-top: 5%;

}
  
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

.img2 {
  position: absolute;
  z-index: -1;
  inset: 0;
  width: 100vw;
  height: 100vh;
  object-fit: contain;
  opacity: 0.03;
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

@media screen and (max-width: 1100px) {

    .img {
      margin-left: inherit
    }
    
    .name-cap {
     
    }
}
</style>