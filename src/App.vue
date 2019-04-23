<template>
  <div id="app">
    <!-- Practice Reference: -->
    <!-- https://i.pinimg.com/736x/e3/af/9c/e3af9c7dc24b3fcb9b5f2d812d839783--cute-pikachu-faces.jpg -->
    <div class="eyes">
      <div class="mouth"></div>
      <div class="lip left"></div>
      <div class="lip right"></div>
    </div>
    <div class="eyeball"></div>
    <div class="cheek"></div>
  </div>
</template>

<script>
export default {
  name: 'app'
}
</script>

<style lang="scss">
body {
  background: #fde644;
}

.eyes {
  width: 380px;
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  margin: auto;
  top: 50px;
  &::before {
    width: 75px;
    height: 75px;
    content: "";
    position: absolute;
    top: 175px;
    left: 0px;
    border-radius: 50%;
    background: #333;
    box-shadow:
      0px 0px 0 0px #333,
      0px 0px 0 0px #333,
      0px 0px 0 0px #333,
      0px 0px 0 0px #333,
      0px 0px 0 5px #333,
      325px 0px 0 0px #333,
      325px 0px 0 5px #333;
  }
}

.eyeball {
  width: 310px;
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  margin: auto;
  top: 150px;
  &::before {
    width: 25px;
    height: 25px;
    content: "";
    position: absolute;
    top: 87px;
    left: 0px;
    border-radius: 50%;
    background: #fff;
    box-shadow:
      0px 0px 0 0px #fff,
      0px 0px 0 0px #fff,
      0px 0px 0 0px #fff,
      0px 0px 0 0px #fff,
      0px 0px 0 5px #fff,
      305px 0px 0 0px #fff,
      305px 0px 0 5px #fff;
  }
}

.cheek {
  width: 430px;
  position: absolute;
  left: 0;
  top: 0;
  right: 0;
  margin: auto;
  top: 250px;
  &::before {
    width: 65px;
    height: 65px;
    content: "";
    position: absolute;
    top: 87px;
    left: 0px;
    border-radius: 50%;
    background: #f71f39;
    box-shadow:
      0px 0px 0 0px #f71f39,
      0px 0px 0 0px #f71f39,
      0px 0px 0 0px #f71f39,
      0px 0px 0 0px #f71f39,
      0px 0px 0 5px #f71f39,
      400px 0px 0 0px #f71f39,
      400px 0px 0 5px #f71f39;
  }
}

.mouth {
  width: 28px;
  height: 14px;
  position: absolute;
  left: 15px;
  top: 10px;
  z-index: 99999;
  right: 0;
  margin: auto;
  bottom: -500px;
  border-radius: 80% 80% 80% 80%;
  background: #333;
}

.lip {
  position: absolute;
  top: 225px;
  right: 73px;
  width: 73px;
  height: 77px;
  border: 4px solid #000;
  border-radius: 50%;
  border-top-color: #fde644;
  background: #fde644;
  &.left {
    left: 125px;
    border-left-color: #fde644;
    border-right-color: #fde644;
    transform: rotate(-23deg);
    &::before {
      top: 2px;
      left: 29px;
    }
  }
  &.right {
    right: 108px;
    border-right-color: #fde644;
    border-left-color: #fde644;
    transform: rotate(15deg);
    &::before {
      top: 2px;
      right: 31px;
    }
  }
}
</style>
