<template>
  <header>
    <HeaderPart />
  </header>
  <body>
    <section>
      <InfosPart />
    </section>
    <section>
      <MainPart />
    </section>
    <footer>
      <FooterPart />
    </footer>
  </body>
</template>

<script>
import HeaderPart from "./components/HeaderPart.vue";
import InfosPart from "./components/InfosPart.vue";
import MainPart from "./components/MainPart.vue";
import FooterPart from "./components/FooterPart.vue";

export default {
  name: "App",
  components: {
    HeaderPart,
    InfosPart,
    MainPart,
    FooterPart,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
*,
*::before,
*::after {
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}
body {
  margin: 0;
}

::-webkit-scrollbar {
  width: 10px;
}

::-webkit-scrollbar-track {
  background: rgba(0, 128, 0, 0.575);
  border-radius: 50px;
}

::-webkit-scrollbar-thumb {
  background: rgb(100, 100, 251);
  border-radius: 50px;
}
</style>
