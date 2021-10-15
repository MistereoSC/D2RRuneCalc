<template>
  <div class="select">
    <div class="items">
      <div class="left">
        <img class="icon" alt="Background" src="../assets/icons/d2logo.png">
        <span>Diablo II</span>
        <img class="icon" alt="Background" src="../assets/icons/dilogo.png">
        <span class="inactive">Diablo Immortal</span>
        
      </div>
      <div class="right">
        <a href="https://ko-fi.com/mistereosc" target="_blank">
          <img class="icon iconlink" alt="Background" src="../assets/icons/KoFi.png">
        </a>
        
        <a href="https://github.com/MistereoSC/D2RRuneCalc" target="_blank">
          <img class="icon iconlink" alt="Background" src="../assets/icons/github.png">
        </a>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Main',
  props: {

  }
}
</script>

<style scoped>
.select {
  position: relative;
  width: 100%;
  height: 30px;
  background-color: #0d0d0d;
  top: 0;
  left: 0;
  user-select: none;

  position: sticky;
  top: 0;
}

.items {
  display: flex;
  height: 30px;
  justify-content: center;
}
.left {
  display: flex;
  max-width: 550px;
  width: 50%;
  min-width: 250px;
}
.right{
  max-width: 550px;
  width: 50%;
  min-width: 200px;
  display: flex;
  justify-content: flex-end;
}
.icon {
  width: 26px;
  height: 26px;
  margin-top: 2px;
  margin-left: 4px;
}
.icon2 {
  width: 20px;
  height: 20px;
  margin-top: 4px;
  margin-left: 8px;
}
.iconlink {
  cursor: pointer;
}
.iconlink:hover{
  filter: brightness(0.5) sepia(1) saturate(10000%) hue-rotate(210deg);
}

span {
  font-family: 'Roboto';
  font-weight: 700;
  font-size: 14px;
  color: #057af0;
  line-height: 30px;
  margin: 0 8px 0 5px;
  padding-top: 1px;
  cursor: default;
}
span.inactive {
  color: #555;
}
</style>
