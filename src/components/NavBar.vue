<template>
    <div class="nav-cont">
<a class="nav" href="mailto:justinp@aevio.com">Email</a>
<router-link to="/about" class="nav">Socials</router-link>
    </div>
</template>

<script setup>

</script>

<style scoped>
.nav-cont {
    position: relative;
    width: 100%;
    height: auto;
    display: flex;
    gap: 5rem;
    inset: 0;
    top: 1%;
    left: -60%;

}

.nav {
    padding: 0;
    align-items: center;
    justify-content: center;
    align-content: center;
    text-align: center;
    grid-row: 1;
    grid-column: 1;
    width: 100%;
    height: max-content;
    font-family: 'raleway', serif;
    color: rgb(105, 105, 105);
    text-shadow: 0px 0px 18px rgb(1, 183, 255);
    font-size: 1.8rem;
  
}
.nav:hover {
    text-shadow: 0px 0px 18px rgb(1, 56, 255);

}
</style>