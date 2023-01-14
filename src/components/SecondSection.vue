<template>
    <div ref="myElement" class="animate-on-scroll img2-cont">
<img src="../assets/DALLE2.png" alt="satoshi" class="img2">
    </div>
    <div class="sub_list">
    <div class="sub_text">Custom Crestron Interfaces</div>
    <div class="sub_text t2">Personalized Control Icons</div>
    <div class="sub_text t3">Integrated Cue Server DMX Projects</div>
    <div class="sub_text t4">Control4 Drivers in Lua Script</div>
  </div>
  <div class="projects">
    <div class="link" v-on:mouseover="showPopup2()">Projects</div>
    <Transition name="fadein">
      <a v-show="showPopup3" class="popup2" href="http://bookofrecipes.netilfy.app">Book Of Recipes</a>
    </Transition>
    <Transition name="fadein">
      <a v-show="showPopup3" class="popup3" href="https://aevio-ch5.netlify.app/">Crestron HTML5</a>
    </Transition>
  </div>
  <div class="link" v-on:mouseover="showPopup1()">Link Up</div>
  <div class="btn_cont_popup">
    <Transition name="fadein" >
  <a   v-show="showPopup" class="popup" href="mailto:justinp@aevio.com">Email</a>
</Transition>
</div>
</template>

<script setup>
import { ref } from 'vue'

const showPopup = ref(false);
const showPopup3 = ref(false);

//funciton to show popup for 5 seconds on mouseover
function showPopup1 () {
setTimeout(() => {
  showPopup.value = true;
}, 300);
setTimeout(() => {
  showPopup.value = false;
}, 5000);
};
function showPopup2 () {
setTimeout(() => {
  showPopup3.value = true;
}, 300);
setTimeout(() => {
  showPopup3.value = false;
}, 5000);
};


</script>

<style scoped>
.img2-cont {
  width: 100%;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 40%;
}

.img2 {
  width: 40vw;
  height: auto;
  object-fit: contain;
  display: flex;
  justify-content: center;
  align-items: center;
  opacity: 0.2;
  border-radius: 40%;
  box-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);
}
 .sub_text {
  font-family: 'raleway', serif;
  font-size: 1.8vw;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  line-height: 5vh;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  padding-top: 5%;
}
 .sub_list {
  padding: 5%;
}
.link {
  font-family: 'raleway', serif;
  font-size: 3vw;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  line-height: 5vh;
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  z-index: 15;
  cursor: pointer;
  max-width: max-content;
  right: -43%;
  margin-top: 30%;
  padding-top: 10%;
  padding-bottom: 10%;
}
.link:hover {
  background-color: rgba(255, 255, 255, 0);
  color: rgb(139, 225, 247);

}

.popup {
  font-family: 'raleway', serif;
  font-size: 3vw;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  line-height: 5vh;
  text-align: center;
  position: absolute;
  bottom: 3rem;
  z-index: 16;
  width: 100%;
  height: auto;
  

}
.popup2 {
  font-family: 'raleway', serif;
  font-size: 3vw;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  line-height: 5vh;
  text-align: center;
  position: absolute;
  bottom: 3rem;
  z-index: 16;
  width: 100%;
  height: auto;
  

}
.popup3 {
  font-family: 'raleway', serif;
  font-size: 3vw;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  line-height: 5vh;
  text-align: center;
  position: absolute;
  bottom: -2rem;
  z-index: 16;
  width: 100%;
  height: auto;
  

}
.popup:hover,.popup2:hover,.popup3:hover {
  background-color: rgba(255, 255, 255, 0);
  color: rgb(139, 225, 247);
  
  
}

.animate-on-scroll.is-animated {
  /* Animate the element sliding in from the left */
  animation: slideInFromLeft 1.5s ease-in-out;
}

@keyframes slideInFromLeft {
  from {
    transform: translateX(-100%);
  }
  to {
    transform: translateX(0);
  }
}
@keyframes fadeIn {
  from { opacity: 0; }
  to { opacity: 1; }
}

</style>