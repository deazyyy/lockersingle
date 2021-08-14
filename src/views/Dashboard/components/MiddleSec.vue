<template>
  <section class="container middlesec">
    <h3 class="heading">CHOOSE YOUR PATH</h3>
    <div class="rowOuter">
      <div class="cols colone">
        <div class="colinner colinnrone">
          <img src="@/assets/img1.png" alt="Logo" class="imges" />
        <h1 class="gradient-text">OLYMPUS <br />DASHBOARD</h1>
        <p>
          Your personal dashboard to manage every aspect of your olympus
          holdings
        </p>
        <button>Explore</button>
        </div>
        
        <img src="@/assets/left.png" alt="Logo" class="leftimg" />
      </div>

      <div class="cols coltwo">
        <div class="colinner colinnrtwo">
          <img src="@/assets/img2.png" alt="Logo" class="imges" />
        <h1 class="gradient-text-blue">LOCKER<br />OF ANANKE</h1>
        <p>
          THE SAFEST PLACE TO LOCK TOKENS AND LIQUIDITY AND EARN REWARDS
        </p>
        <button>Explore</button>
        </div>
        <img src="@/assets/right.png" alt="Logo" class="rightimg" />
      </div>
    </div>
  </section>
</template>

<script>
// @ is an alias to /src
export default {
  name: "MiddleSec",
};
</script>

<style scoped>

.middlesec{
  min-height: 70vh;
}
.cols button{
  position: absolute;
  left: 50%;
  transform: translate(-50%,-50%);
  border:0;
  padding: 6px 24px;
  background: transparent;
  border-radius: 24px;
  z-index: 5;
  bottom: -30px;
  color: #fff;
  font-weight: 600;
  text-transform: uppercase;
}
.colinnrone button{
  background:linear-gradient(to right, #f74541 0%, #f7c347 100%)
}
.colinnrtwo button{
  background:linear-gradient(to right, #3345f5 0%, #3bc9f5 100%)
}
.colone:hover{
  box-shadow:0px 0px 45px 10px rgba(247, 195, 71, 0.3);  
}
.colinnrone{
  position: relative;
  padding-bottom: 24px;
}
.colinnrone:before{
  position: absolute;
  width: calc(100% + 40px );
  height: 5px;
  bottom: 0;
  left: -20px;
  background: linear-gradient(to right,transparent 0%, #f74541 7%,  #f7c347 93%, transparent 100%);;
  z-index: 1;
  content:""
}
.colinnrtwo{
  position: relative;
  padding-bottom: 24px;
}
.colinnrtwo:before{
  position: absolute;
  width: calc(100% + 40px );
  height: 5px;
  bottom: 0;
  left: -20px;
  background: linear-gradient(to right,transparent 0%, #3345f5 7%,  #3bc9f5 93%, transparent 100%);;
  z-index: 1;
  content:""
}
.coltwo:hover{
  box-shadow:0px 0px 45px 10px rgba(59, 201, 245, 0.3);  
}
.leftimg{
  position: absolute;
  left: 0;
  height: 78%;
  width: auto;
  top: 18%;
}
.rightimg{
  position: absolute;
  right: 0;
  height: 78%;
  width: auto;
  top: 18%;
}
.rightimg, .leftimg{
  opacity: 0.5;
      z-index: -2;
      pointer-events: none;
}
.heading{
  text-align: center;
}
.rowOuter{
  display: flex;
  justify-content:center;
  margin-top: 140px;
}
.cols {
  background-color: #081a2e;
  padding: 24px;
  border-radius: 18px;
  text-align: center;
  margin: 0 36px;
  max-width: 500px;
  padding-bottom: 0;
  cursor: pointer;
      min-width: 420px;
}
.cols h1 {
  font-size: 30px;
}
.cols p {
  font-size: 18px;
  text-transform: uppercase;
}
.cols .imges {
  height: 160px;
  width: auto;
  display: block;
  margin: auto;
  position: absolute;
  left: 50%;
  transform: translateX(-50%);
  top: -100px;
  
}
.colinner {
margin-top: 0px;
height: 100%;
padding-top: 80px;
}


.rowOuter:hover > * {
  opacity: 0.5;
  transition: all 0.3s ease;
}

.rowOuter:hover > *:hover {
  opacity: 1;
}
.rowOuter:hover > *:hover img{
  opacity: 1;
}
@media screen and (max-width: 1550px) {
  .cols{
    max-width: 400px;
    min-width: unset;
  }
}
@media screen and (max-width: 1300px) {
  .cols{
    max-width: 350px;
    min-width: unset;
  }
}
@media screen and (max-width: 1200px) {
  .rightimg, .leftimg{
 height: 60%;
}
}
@media screen and (max-width: 1070px) {
  .rowOuter{
    flex-direction: column;
    margin-top: 30px;
  }
  .cols{
    max-width: unset;
    margin-top: 140px;
  }
  .rightimg, .leftimg{
    display: none;
  }
}
@media screen and (max-width: 600px) {
  .rowOuter{
    margin-top: 20px;
  }
  .cols{
    max-width: unset;
    min-width: unset;
    margin: 0;
    margin-top: 140px;
  }
}
</style>
