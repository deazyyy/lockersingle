<template>
  <section class="container bottomcont">
    <div class="row">
      <div class="col-md-6 wow fadeInLeft"
        data-wow-duration="0.6s"
        data-wow-delay="1.6s">
        <div class="infoBox">
          <div class="gradient-text">
            GAIN FAVOUR FROM THE GODS - 9 DAILY TASKS
          </div>
          <div class="info">
            <div>⚡️Do these to invoke favour from the Gods of Olympus⚡️</div>
            <div>
              <span>1.</span> Bogged.Charts - Click 'Heart' on Olympus Icon
              (Visit at least once every 8 hours to give an upvote on the
              backend) <br />
              <a href="https://charts.bogged.finance/0x18b426813731C144108c6D7FAf5EdE71" target="_blank">https://charts.bogged.finance/0x18b426813731C144108c6D7FAf5EdE71</a>
            </div>
            <div>
              <span>2.</span>Twitter - Like, Retweet & Comment on every new
              post<br />
              <a href="https://twitter.com/olympus_token" target="_blank">https://twitter.com/olympus_token</a>
            </div>
            <div>
              <span>3.</span>Instagram - Like & comment on every new post<br />
              <a href="https://www.instagram.com/olympusbsc/?hl=en" target="_blank">https://www.instagram.com/olympusbsc/?hl=en</a>
            </div>
            <div>
              <span>4.</span>Coinmarketcap - Add to Watchlist<br />
              <a href="https://coinmarketcap.com/currencies/olympus-token/" target="_blank">https://coinmarketcap.com/currencies/olympus-token/</a>
            </div>
            <div>
              <span>5.</span>Coingecko - Click Like<br />
              <a href="https://www.coingecko.com/en/coins/olympus-token" target="_blank">https://www.coingecko.com/en/coins/olympus-token</a>
            </div>
            <div>
              <span>6.</span>CoinSniper - Vote <br />
              <a href="https://coinsniper.net/coin/4469" target="_blank">https://coinsniper.net/coin/4469</a>
            </div>
            <div>
              <span>7.</span>CoinHunt - Click all the positive emojis<br />
              <a href="https://coinhunt.cc/coin/1375929387" target="_blank">https://coinhunt.cc/coin/1375929387</a>
            </div>
            <div>
              <span>8.</span> Coinbase - Add to Watchlist<br />
              <a href="https://www.coinbase.com/price/olympus-token" target="_blank">https://www.coinbase.com/price/olympus-token</a>
            </div>
            <div>
              <span>9.</span>Reddit - Upvote, Comment and Award the latest
              post<br />
             <a href="https://www.reddit.com/search/?q=Olympus%20token" target="_blank">https://www.reddit.com/search/?q=Olympus%20token</a>
            </div>
          </div>
        </div>
      </div>
      <div class="col-md-6  wow fadeInRight"
        data-wow-duration="0.6s"
        data-wow-delay="1.6s">
        <div class="zeuslogoOuter">
          <img src="@/assets/zeus.png" alt="Logo" class="zeuslogo" />
        </div>
      </div>
    </div>
    <pseudo-window
			@resize.passive="onResize" />
  </section>
  
</template>

<script>
// @ is an alias to /src
// import ItemComp from "@/components/Itemc.vue";
import PseudoWindow from 'vue-pseudo-window';
export default {
  name: "Bottom",
  components: {
		PseudoWindow
	},
  mounted: function() {
        document.querySelector(".zeuslogo").style.maxHeight = document.querySelector(".infoBox").offsetHeight +"px"
    },
  methods: {
		onResize() {
      let height = document.querySelector(".infoBox").offsetHeight
      document.querySelector(".zeuslogo").style.maxHeight = height+"px";
		}
	}
};
</script>

<style scoped>
.infoBox {
  border-radius: 16px;
  background-color: #081a2e;
  padding: 30px 20px;
}
.gradient-text {
  text-align: center;
}
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
.info div {
  margin: 20px 0;
  text-align: center;
}
.info a{
  word-break: break-all;
  color: #fff;
}
.info a:hover{
  text-decoration: underline;
}
.info span {
  color: #f7c347;
  padding-right: 10px;
}

.zeuslogoOuter {
  display: flex;
  justify-content: center;
  align-items: center;
}
.zeuslogo {
  height: 100%;
  width: auto;
  max-height: 80vh;
  max-width: 90%;
}
@media screen and (max-width: 1100px) {
  .bottomcont .row{
    flex-direction: column;
  }
  .bottomcont .col-md-6{
    max-width: 100%;
  }
  .zeuslogo{
    max-width: 30vw;
  }
}
@media screen and (max-width: 650px) {
  .zeuslogoOuter {
    display: none !important;
  }
  .info div {
    font-size: 14px;
  }
  .col-md-6 {
    padding: 0;
  }
  .infoBox {
    border-radius: 0 !important;
  }
  .bottomcont {
    width: 100%;
    border-width: 3px;
    border-style: solid;
    position: relative;
    border-right: 0 !important;
    border-left: 0 !important;

    border-image: linear-gradient(to right, #f74541, #f7c347) 100% 1;
  }

  .bottomcont::after {
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
}
</style>
