<template>
    <div id="diamond">

    </div>
    <Star/>
</template>

<script>
import Star from "./testing2"
export default {
components:{
    Star
}
}
</script>

<style scoped>
  #diamond {
      width: 0;
      height: 0;
      border: 50px solid transparent;
      border-bottom-color: red;
      position: relative;
      top: -50px;
    }
    #diamond:after {
      content: '';
      position: absolute;
      left: -50px;
      top: 50px;
      width: 0;
      height: 0;
      border: 50px solid transparent;
      border-top-color: red;
    }
</style>