<template>
  <div>
    <div class="wave-animation"></div>
  </div>
</template>

<style scoped>
.wave-animation {
  height: 198px;
  background: url('../../assets/wave-sketch.svg') repeat-x;
  animation: wave 25s cubic-bezier(0.36, 0.45, 0.63, 0.53) infinite;
  transform: translate3d(0, 0, 0);
}
@media only screen and (max-width: 768px) {
  .wave-animation {
    animation: wave 20s cubic-bezier(0.36, 0.45, 0.63, 0.53) infinite;
  }
}
@keyframes wave {
  0% {
    margin-left: -1600px;
  }
  100% {
    margin-left: 0;
  }
}
</style>
