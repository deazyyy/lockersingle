<template>
  <div>
    <Navbar />
    <MiddleSec/>
    <Footer />
  </div>
</template>

<script>
// @ is an alias to /src
import Navbar from "./components/Navbar.vue";
import MiddleSec from "./components/MiddleSec.vue";

import Footer from "./components/Footer.vue";
export default {
  name: "Apps",
  components: {
    Navbar,
    MiddleSec,
    Footer,
  },
};
</script>
