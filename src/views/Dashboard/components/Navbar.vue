<template>
<div class="wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="0.5s">
  <nav  >
    <img src="@/assets/logon.png" alt="Logo" class="logo" />
    <div class="left">
      <div class="icons">
        <div class="val-bg">
          <img src="@/assets/circle.png" alt="Logo" class="logo" />
          $ 0.00000344265
        </div>

        <div class="socialIcons">
          <a href="https://mobile.twitter.com/olympus_token" target="_blank"><i class="fab fa-twitter"></i></a>
          <a href="https://www.instagram.com/olympusbsc/?hl=en" target="_blank"><i class="fab fa-instagram"></i></a>
          <a href="https://t.me/OlympusOfficial" target="_blank"><i class="fab fa-telegram"></i></a>
          <a href="mailto:contact@olympustoken.io" target="_blank"><i class="fas fa-envelope"></i></a>
        </div>
      </div>
      <!-- <Button name="Connect" class="connectBtn"/> -->
    </div>
  </nav>
  </div>
</template>

<script>
// @ is an alias to /src
// import Button from "@/components/Button.vue";
export default {
  name: "Navbar",
  // components: {
  //   Button,
  // }
};
</script>

<style scoped>
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background: #081a2e;
  padding: 10px 30px;
  position: relative;
  /* border-bottom: linear-gradient(to right, #f74541, #f7c347); */
  border-width: 3px;
  border-style: solid;
  border-top: 0 !important;
  border-image: linear-gradient(to right, #f74541, #f7c347) 100% 1;
}
nav::after {
  position: absolute;
  content: "";
  width: 100%;
  height: 100%;
  right: 0;
  left: 0;
  top: 0;
  background: linear-gradient(to right, #f74541, #f7c347);
  filter: blur(10px);
  z-index: -1;
}
nav .logo {
  width: auto;
  max-height: 40px;
}
.left,
.icons {
  display: flex;
  align-items: center;
}
.val-bg {
  border-radius: 100px;
  background-color: #25364d;
  display: flex;
  align-items: center;
  padding: 3px 14px 3px 0;
}
.val-bg img {
  width: 40px;
  height: auto;
  margin-right: 10px;
}
.socialIcons {
  margin: 0 14px;
}
.socialIcons i {
  margin: 0 5px;
  color: #c4c7cb;
  cursor: pointer;
}
.socialIcons i:hover {
  color: #fff;
}
@media screen and (max-width: 991px) {
  nav .logo {
    max-height: 30px;
  }
  .val-bg {
    font-size: 14px;
    padding: 3px ;
    margin-left: 10px;
  }
  .val-bg img {
        width: auto;
    height: 100%;
  }
}
@media screen and (max-width: 768px) {
  nav .logo {
    max-height: 30px;
  }
  .val-bg {
    font-size: 14px;
    padding: 5px 14px;
    margin: 0 10px;
  }
  .val-bg img {
       width: auto;
    height: 100%;
  }
  .socialIcons {
    display: none;
  }
}
@media screen and (max-width: 650px) {
  .val-bg {
    display: none;
  }
  nav .logo {
    max-height: 30px;
  }
}
@media screen and (max-width: 500px) {
    nav{
        padding: 10px 14px;
    }
  nav .logo {
    max-height: unset;
    width: 60%;
    height: auto;
  }
}
</style>
