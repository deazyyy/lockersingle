<template>
  <section class="container" >
    <div class="holdersBx wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="1.2s">
      TOTAL PAID TO HOLDERS
      <div style="display:flex;align-items: flex-end;">
        <h2 class="gradient-text">2,216,144,315.16</h2>
        BUSD
      </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src
// import ItemComp from "@/components/Itemc.vue";
export default {
  name: "Holders",
};
</script>

<style scoped>
.holdersBx {
  display: flex;
  align-items: center;
  font-size: 22px;
  background: #081a2e;
  padding: 20px 40px;
  vertical-align: middle;
  justify-content: center;
  border-radius: 16px;
}
.holdersBx .gradient-text {
  font-size: 40px;
  margin: 0 30px;
}

@media screen and (max-width: 850px) {
  .holdersBx {
    font-size: 18px;
  }
  .holdersBx .gradient-text {
    font-size: 30px;
  }
}
@media screen and (max-width: 650px) {
  .gradient-text {
    margin: 0 !important;
    margin-right: 5px !important;
  }
  .holdersBx {
    font-size: 16px;
  }
  .holdersBx .gradient-text {
    font-size: 28px;
  }
  .holdersBx {
    flex-direction: column-reverse;
  }
}
@media screen and (max-width: 500px) {
  .holdersBx {
    font-size: 16px;
  }
  .holdersBx .gradient-text {
    font-size: 24px;
  }
}
</style>
