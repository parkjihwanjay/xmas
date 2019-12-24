<template>
  <div id="app">
    <div id="heart">
      <img class="heart-img" src="/img/couple.png" alt="지환 수빈 커플">
      <!-- <img class="heart-img" src="https://upload.wikimedia.org/wikipedia/commons/c/c8/Love_Heart_symbol.svg" alt="수빈이에 대한 사랑"> -->
    </div>
    <div id="footer">
      <div class="xmas-tree">
        <img class="xmas-tree-img" src="https://image.flaticon.com/icons/png/512/2367/2367639.png" alt="트리~">
      </div>
      <div class="couple">
        <img class="heart-img" src="https://upload.wikimedia.org/wikipedia/commons/c/c8/Love_Heart_symbol.svg" alt="수빈이에 대한 사랑">
        <!-- <img class="xmas-tree-img" src="/img/couple.png" alt="트리~"> -->
      </div>
      <div class="xmas-tree">
        <img class="xmas-tree-img" src="https://image.flaticon.com/icons/png/512/2367/2367639.png" alt="트리~">
      </div>
    </div>
    <Snow color="white"/>
  </div>
</template>

<script>
import Snow from 'vue-niege';

export default {
  name: 'app',
  components: {
    Snow,
  }
}
</script>

<style>
#app{
  width : 100%;
  min-height: 604px;
}
#heart{
  width : 307px;
  height : 314px;
  margin : 0 auto;
  margin-top : 100px;
  /* position: absolute;
  top : 50%;
  left : 50%;
  transform : translate(-50%, -50%); */
  /* animation : pulse 1s ease infinite; */
}
.heart-img{
  width : 100%;
  height : 100%;
}

@keyframes pulse {
  0% { transform: scale(1); }
  50% { transform: scale(1.2); }
  100% { transform: scale(1); }
}

#footer{
  width : 100%;
  display: flex;
  justify-content: space-between;
  position:absolute; 
  bottom:0px;
}

.xmas-tree{
  width : 200px;
  height : 200px;
}
.xmas-tree-img{
  width : 100%;
  height: 100%;
}

.couple{
  width : 200px;
  height: 200px;
  animation : pulse 1s ease infinite;
  margin-bottom: 20px;
}
</style>
