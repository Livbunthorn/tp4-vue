<template>
<h1>I'm the root component</h1>
<br>
<div class="wrapper">
<Traingle/>
<Hexagon/>
<Heart/>

<Diamond/>
<Star/>
</div>

</template>

<script>

import Traingle from "./components/Triangle"
import Hexagon from "./components/Hexagon"
import Heart from "./components/Heart"
import Diamond from "./components/Diamond"
import Star from "./components/Star"
export default {
  name: 'App',
  components: {
    Traingle,
    Hexagon,
    Heart,
    Diamond,
    Star
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.wrapper{
  display: flex;
  justify-content: space-between;
}
.diamond{
  color: yellow;
}
</style>
