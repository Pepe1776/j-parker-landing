<template>
    <div class="img2-cont">
<img src="../assets/SAtoshi_art.png" alt="satoshi" class="img2">
    </div>
    <div class="sub_list">
    <div class="sub_text">Custom Crestron Interfaces</div>
    <div class="sub_text t2">Personalized Control Icons</div>
    <div class="sub_text t3">Integrated Cue Server DMX Projects</div>
    <div class="sub_text t4">Control4 Drivers in Lua Script</div>
  </div>
</template>

<script setup>
    
</script>

<style scoped>
.img2-cont {
width: 100vw;
height: 100vh;
inset: 0;
}

.img2 {
  width: 40%;
  height: auto;
  object-fit: contain;
  position: absolute;
  left: -30%;
  bottom: 5%;
  opacity: 0.2;
  border-radius: 40%;
  box-shadow: -5px 5px 18px rgba(1, 161, 224, 0.75);
}
 .sub_text {
  font-family: 'raleway', serif;
  font-size: 1.8rem;
  color: rgb(105, 105, 105);
  text-shadow: 0px 0px 25px rgb(1, 183, 255);
  line-height: 5rem;
}
 .sub_list {
 position: absolute;
 left: 20%;
 bottom: 15%;
}
</style>