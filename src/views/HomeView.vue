<template>
  <div class="home">
    <div class="home">
      <h1 class="heading">
          Rooted Retreat <br>
           "Planting Happiness, One Leaf at a Time."
        </h1>
  </div>
</div>
<About/>
<Featured/>
</template>

<script>
import Home from '@/components/Home.vue'
import About from '@/components/About.vue'
import Featured from '@/components/Featured.vue'
  export default {
    components: {
      Home,
      About,
      Featured
    }
  }
</script>

<style scoped>
.home{
  background-image: url(https://i.postimg.cc/zBpSw6vx/prudence-earl-Nw-Bx723-Xa-Hw-unsplash.jpg) !important;
      position:relative;
      background-size: cover;
      height: 110vh;
      width: 100%;
  }

  .heading {
    color: rgb(119, 210, 119);
    text-shadow: 2px 2px white;
    position: absolute;
    display: flex !important;
    justify-content: start !important;
    max-width: 460px;
    top: 21rem;
    left: 3rem;
    font-weight: bold;
}
</style>
