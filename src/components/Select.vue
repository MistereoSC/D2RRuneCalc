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
}

.items {
  margin-left: max(calc(50% - 600px), 0px);
  display: flex;
  height: 30px;
}
.left {
  display: flex;
  max-width: 600px;
  width: 50%;
  min-width: 300px;
}
.right{
  max-width: 600px;
  width: 50%;
  min-width: 300px;
  display: flex;
  justify-content: flex-end;
}
.icon {
  width: 26px;
  height: 26px;
  margin-top: 2px;
  margin-left: 4px;
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
