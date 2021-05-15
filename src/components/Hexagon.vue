<template>
<div>
  
</div>
    <div id="hexagon" >
  
    </div>
    <div id="heart">
        <Heart/>
    </div>
 
</template>

<script>
import Heart from "./testing"
export default {
    components:{
      Heart
    },
    data(){
      return{
        color:"blue"
      }
    }
}
</script>

<style >
#heart{
  color: yellow;
}
 #hexagon {
  width: 100px;
  height: 57.735px;
  background: blue;
  position: relative;
}
#hexagon::before {
  content: "";
  position: absolute;
  top: -28.8675px;
  left: 0;
  width: 0;
  height: 0;
  border-left: 50px solid transparent;
  border-right: 50px solid transparent;
  border-bottom: 28.8675px solid blue;
}
#hexagon::after {
  content: "";
  position: absolute;
  bottom: -28.8675px;
  left: 0;
  width: 0;
  height: 0;
  border-left: 50px solid transparent;
  border-right: 50px solid transparent;
  border-top: 28.8675px solid blue;
}
</style>