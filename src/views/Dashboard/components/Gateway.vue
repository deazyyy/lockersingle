<template>
  <section class="container">
    <h3 class="heading wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="0.3s">YOUR GATEWAY TO OLYMPUS</h3>
    <div class="row">   
      <div class="col-md-3 wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="0.45s" >
        <div class="card-header">
          <img src="@/assets/c1.svg" alt="Logo" class="card-header_img" />
          <div class="card-header_center">
            <h2 class="gradient-text">2,216,144,315.16</h2>
            <h2 class="gray">~ $2,893</h2>
          </div>
          <h3 class="card-header_btm">TOTAL OLYMPUS HOLDINGS</h3>
        </div>
        <Button name="BUY OLYMPUS" />
      </div>
      <div class="col-md-3  wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="0.6s">
        <div class="card-header">
          <img src="@/assets/c2.svg" alt="Logo" class="card-header_img" />
          <div class="card-header_center d-flex">
            <h2 class="gradient-text mr-2">1,282</h2>
            <div style="font-size:14px;vertical-align:middle">BUSD</div>
          </div>
          <h3 class="card-header_btm">TOTAL BUSD HOLDINGS</h3>
        </div>
        <Button name="approve busd" class="bb-btn"/>
        <div class="approve_ip">

                <ul class="nav nav-pills ip_values" role="tablist">
    <li class="nav-item">
      <a class="nav-link active" data-toggle="pill" href="#home">25%</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" data-toggle="pill" href="#menu1">50%</a>
    </li>
    <li class="nav-item">
      <a class="nav-link" data-toggle="pill" href="#menu2">75%</a>
    </li>
     <li class="nav-item">
      <a class="nav-link" data-toggle="pill" href="#menu2">100%</a>
    </li>
  </ul>
  
          <div class="ipOuter">
            <input />
            <span>BUSD</span>
          </div>
        </div>
        <Button name="Re-invest busd"/>
      </div>
      <div class="col-md-3  wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="0.75s">
        <div class="card-header">
          <img src="@/assets/c3.svg" alt="Logo" class="card-header_img" />
          <div class="card-header_center">
            <h2 class="gradient-text">2 Hours 3 Mins Ago</h2>
          </div>
          <h3 class="card-header_btm">PREVIOUS PAYOUT TIME</h3>
        </div>
        <Button name="Claim 1,282 BUSD" class="bb-btn"/>
        <div class="info">
          Places a small transaction to trigger <br />
          (less than $0.10)
        </div>
      </div>
      <div class="col-md-3  wow fadeInDown"
        data-wow-duration="0.6s"
        data-wow-delay="0.9s">
        <div class="card-header">
          <img src="@/assets/c4.svg" alt="Logo" class="card-header_img" />
          <div class="card-header_center">
            <h2 class="gradient-text">14%</h2>
          </div>
          <h3 class="card-header_btm">CURRENT HADES SELL TAX</h3>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src
import Button from "@/components/Button.vue";
export default {
  name: "Gateway",
  components: {
    Button,
  }
}
</script>

<style scoped>
.heading {
  font-weight: 600;
  margin-bottom: 40px;
  text-align: center;
}
.cardRow {
  display: flex;
  justify-content: center;
  /* margin:  0 -8px; */
}
/* .col-md-3{
    margin: 0 10px;
} */
.info {
  color: #bfc3c9;
  text-align: center;
  font-size: 13px;
  margin-top: 8px;
}
.col-md-3 .btn-main {
  width: auto;
}
.card-header {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  background-color: #081a2e;
  border-radius: 20px;
  padding: 16px 20px;
  align-items: center;
  text-align: center;
  margin-bottom: 14px;
  /* height: 100%; */
  min-height: 210px;
  position: relative;
}
.card-header_img {
  height: 70px;
  width: auto;
}
.card-header h2,
.card-header h3 {
  margin: 0;
  font-weight: 600;
letter-spacing: 0.4pt;
}
h3 {
  font-size: 18px;
}
h2 {
  font-size: 24px !important;
}
.card-header_center {
  margin: 7px 0;
}

/* second card */
.approve_ip {
  margin: 8px 0 14px;
}
.ipOuter input{
    width: 100% !important;
    padding-left: 14px;
    padding-right: 30px;
    position: relative;
width: 110px;
height: 45px;
margin-left: auto;
margin-right: auto;
overflow: hidden;
transition: 0.5s;
color: #ffff;
font-size: 13px;
border-radius: 30px;
background: #39475c;
 border: 2px solid #6f7c8e;
  outline: none;
}
.ipOuter input:focus {
  border: 2px solid #6f7c8e;
  outline: none;
}
.ipOuter input:hover {
  background: #39475c;
  border: 2px solid #6f7c8e;
}
.ipOuter{}
.ipOuter {
  position: relative;
}
.ipOuter span {
  position: absolute;
  right: 20px;
  top: 50%;
  transform: translateY(-48.5%);
  font-size: 14px;
}
.ip_values {
  display: flex;
  justify-content: space-between;
  margin: 2px 14px 6px;
}
.ip_values{
    
}
.ip_values a{
    color: #fff;
    background: transparent;
    padding: 0;
}
.ip_values .active {
    background: transparent;
    color:#f7c347;
    font-weight: 700;
}
.ip_values span {
  font-size: 12px;
}
@media screen and (max-width: 991px) {
  h2 {
    font-size: 20px !important;
  }
  h3 {
    font-size: 15px !important;
  }
}
@media screen and (max-width: 850px) {
  h2 {
    font-size: 18px !important;
  }
  h3 {
    font-size: 14px !important;
  }
}
@media screen and (max-width: 768px) {
  h2 {
    font-size: 18px !important;
  }
  h3 {
    font-size: 14px !important;
  }
  .col-md-3:not(:last-child) {
    margin-bottom: 50px;
  }
}

@media screen and (max-width: 650px) {
  h2 {
    font-size: 18px !important;
  }
  h3 {
    font-size: 14px !important;
  }
  .col-md-3:last-child .card-header {
    align-items: center;
    text-align: center;
  }
  .col-md-3:last-child .card-header .gradient-text {
    font-size: 24px !important;
  }
  .col-md-3 {
    padding-left: 40px;
    position: relative;
    padding-bottom: 40px;
    margin-bottom: 40px !important;
  }
  .col-md-3::after {
    position: absolute;
    content: "";
    width: 60%;
    height: 3px;
    right: 0;
    left: 50%;
    bottom: 0;
    transform: translateX(-50%);
    border-radius: 3px;
    background-color: #4c5d74;
    z-index: -1;
  }
  .card-header {
    min-height: unset;
    padding: 26px 20px;
    /* align-items: flex-end;
    text-align: right; */
  }
  .card-header_img {
    position: absolute;
    left: 0;
    top: 50%;
    transform: translate(-50%, -50%);
    width: auto;
    height: 80%;
    max-height: 50px;
    min-height: 40px;
  }
}
</style>
