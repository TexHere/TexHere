<template>
  <div :class="$style.App">
    <div :class="$style.Header">
      Welcome to 
    <div :class="$style.logo"><span><svg xmlns="http://www.w3.org/2000/svg" style="height: 14rem;margin-right: 0;" viewBox="0 0 512 512"><!--! Font Awesome Pro 6.0.0 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path fill="currentColor" d="M176 256C176 211.8 211.8 176 256 176C300.2 176 336 211.8 336 256C336 300.2 300.2 336 256 336C211.8 336 176 300.2 176 256zM256 0C273.7 0 288 14.33 288 32V66.65C368.4 80.14 431.9 143.6 445.3 224H480C497.7 224 512 238.3 512 256C512 273.7 497.7 288 480 288H445.3C431.9 368.4 368.4 431.9 288 445.3V480C288 497.7 273.7 512 256 512C238.3 512 224 497.7 224 480V445.3C143.6 431.9 80.14 368.4 66.65 288H32C14.33 288 0 273.7 0 256C0 238.3 14.33 224 32 224H66.65C80.14 143.6 143.6 80.14 224 66.65V32C224 14.33 238.3 0 256 0zM128 256C128 326.7 185.3 384 256 384C326.7 384 384 326.7 384 256C384 185.3 326.7 128 256 128C185.3 128 128 185.3 128 256z"/></svg></span><span>TexHere</span></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'WelcomeComponent'
}
</script>
<style lang="scss" scoped module>
@keyframes Welcome {
  0% {
    opacity: 0;
    margin-right: 6rem;
  }
  100% {
    opacity: 1;
    margin-right: 0;
  }
}
@keyframes Logo {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
  .App {
    display: flex;
    justify-content: center;
    width: 100%;
    height: 100%;
    .Header {
      position: absolute;
      display: flex;
      justify-content: center;
      align-items: center;
      top: 30%;
      font-size: 4.5rem;
      color: #e5e9f0;
      font-family: 'Poppins', sans-serif;
      animation: Welcome 3s ease;
      height: 16rem;
    }
    .logo {
      display: flex;
      flex-direction: column;
      // position: absolute;
      // bottom: 30%;
      // transform: translate(50%, 50%)
      span svg {
        color: #e5e9f0;
        animation: Logo 3s ease;
      }
    }
  }


</style>
