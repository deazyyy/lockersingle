<template>
  <nav class="wow fadeInDown" data-wow-duration="0.6s" data-wow-delay="0.6s">
    <div class="socialIcons">
      <a href="https://mobile.twitter.com/olympus_token" target="_blank"
        ><i class="fab fa-twitter"></i
      ></a>
      <a href="https://www.instagram.com/olympusbsc/?hl=en" target="_blank"
        ><i class="fab fa-instagram"></i
      ></a>
      <a href="https://t.me/OlympusOfficial" target="_blank"
        ><i class="fab fa-telegram"></i
      ></a>
      <a href="mailto:contact@olympustoken.io" target="_blank"
        ><i class="fas fa-envelope"></i
      ></a>
    </div>
  </nav>
</template>

<script>
// @ is an alias to /src
// import ItemComp from "@/components/Itemc.vue";
export default {
  name: "Footer",
};
</script>

<style scoped>
nav {
  display: flex;
  justify-content: center;
  padding: 10px 30px 50px;
}

.socialIcons {
  display: flex;
  margin: 0 14px;
}
.socialIcons a {
  margin: 0 10px;
  border-radius: 50%;
  border: 2px solid #334455;
  padding: 10px;
  width: 50px;
  height: 50px;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: all 0.3s ease;
  cursor: pointer;
}
.socialIcons a:hover {
  background: #334455;
}
.socialIcons i {
  margin: 0 1px;
  color: #c4c7cb;
  font-size: 22px;
}
</style>
