<template>
  <div>
    <Navbar />
    <Gateway />
    <Holders />
    <Bottom />
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "./components/Navbar.vue";
import Gateway from "./components/Gateway.vue";
import Holders from "./components/Holders.vue";
import Bottom from "./components/Bottom.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "Dashboard",
  components: {
    Navbar,
    Gateway,
    Holders,
    Bottom,
    Footer,
  },
};
</script>
