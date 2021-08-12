<template>
  <Apps />
</template>

<script>
import Apps from "@/views/Dashboard/Apps.vue";

export default {
  name: "App",
  components: {
    Apps,
  },
};
</script>

<style>
* {
  font-family: "Open Sans", sans-serif;
}
body {
  background-color: #1a293e;
  font-family: "Open Sans", sans-serif;
  color: #fff;
  margin: 0;
}
section.container {
  margin-top: 50px;
  margin-bottom: 50px;
}

.gradient-border {
  background: linear-gradient(to right, #3345f5 0%, #3bc9f5 100%) !important;
  border-radius: 50px;
  padding: 14px;
  position: relative;
  z-index: 1;
}
.gradient-border::before {
  position: absolute;
  content: "";
  width: calc(100% - 6px);
  height: calc(100% - 6px);
  top: 3px;
  left: 3px;
 border-radius: 50px;
  background-color: #273f59;
  z-index: -1;
}

.gradient-text {
    background: linear-gradient(to right, #f74541 0%, #f7c347 25%, #f74541 50%, #f7c347 75%, #f74541 100%);

  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 700 !important;
   background-size: 400%;
  animation: hue 10s infinite linear;
}

.gradient-text-blue{
   background: linear-gradient(to right, #3345f5 0%, #3bc9f5 25%, #3345f5 50%, #3bc9f5 75%, #3345f5 100%);

  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-weight: 700 !important;
   background-size: 400%;
  animation: hue 10s infinite linear;
}
@-webkit-keyframes hue {
  0% {
    background-position: 0%;
  }
  100% {
    background-position: 400%;
  }
}
.gray {
  color: #97a0ad;
}

.container {
  max-width: 1600px;
  margin: auto;
}

@media screen and (max-width: 650px) {
  .container {
    width: 86%;
    margin: auto;
  }
}
@media screen and (max-width: 500px) {
  .container {
    width: 95%;
    margin: auto;
  }
}
</style>
