<template>
    <div class="img2-cont">
<img src="../assets/DALLE2.png" alt="satoshi" class="img2">
    </div>
    <div class="sub_list">
    <div class="sub_text">Custom Crestron Interfaces</div>
    <div class="sub_text t2">Personalized Control Icons</div>
    <div class="sub_text t3">Integrated Cue Server DMX Projects</div>
    <div class="sub_text t4">Control4 Drivers in Lua Script</div>
  </div>
  <a class="link" href="mailto:justinp@aevio.com">Link Up</a>
</template>

<script setup>
    
</script>

<style scoped>
.img2-cont {
  width: 100%;
  height: auto;
  display: flex;
  justify-content: center;
  align-items: center;
  margin-top: 10%;
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
  z-index: 5;
  cursor: pointer;
  max-width: max-content;
  right: -43%;
  padding-top: 10%;
  padding-bottom: 10%;
}
.link:hover {
  background-color: rgba(255, 255, 255, 0);

}
</style>