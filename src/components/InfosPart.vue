<template>
  <div class="background">
    <img id="myPic" src="@/assets/myPic.jpg" alt="Selfhtml" />
    <h3>Filters</h3>
    <section class="filter">
      <div class="sepiaFilter">
        <p>sepia</p>
        <input
          @input="sepiaFilter"
          type="range"
          name=""
          id="sepia"
          min="0"
          max="100"
          v-model="sepia"
        />
        <p>{{ sepia }}%</p>
      </div>
      <div class="grayFilter">
        <p>grayscale</p>
        <input
          @input="grayscaleFilter"
          type="range"
          name=""
          id="grayscale"
          min="0"
          max="100"
          v-model="grayscale"
        />
        <p>{{ grayscale }}%</p>
      </div>
      <div class="invertFilter">
        <p>inviert</p>
        <input
          @input="invertFilter"
          type="range"
          name=""
          id="invert"
          min="0"
          max="100"
          v-model="invert"
        />
        <p>{{ invert }}%</p>
      </div>
    </section>
    <div class="center">
      <p>Visit My Githube Profil</p>
      <a href="https://github.com/BringsCoding" target="_blank"
        ><img alt="W3Schools" src="@/assets/GitHub-Mark-Light-64px.png"
      /></a>
      <h2>Simon Brings</h2>
      <p>25 years old from germany</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      sepia: 0,
      grayscale: 0,
      invert: 0,
    };
  },
  methods: {
    sepiaFilter() {
      const img = document.querySelector("#myPic");

      const GrayFilter = document.querySelector("#sepia");

      GrayFilter.addEventListener("input", function (e) {
        img.style.setProperty("--sepia", e.target.value + "%");
      });
    },
    grayscaleFilter() {
      const img = document.querySelector("#myPic");

      const GrayFilter = document.querySelector("#grayscale");

      GrayFilter.addEventListener("input", function (e) {
        img.style.setProperty("--grrayscale", e.target.value + "%");
      });
    },
    invertFilter() {
      const img = document.querySelector("#myPic");

      const GrayFilter = document.querySelector("#invert");

      GrayFilter.addEventListener("input", function (e) {
        img.style.setProperty("--invert", e.target.value + "%");
      });
    },
  },
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Staatliches&display=swap");

* {
  text-align: center;
  font-family: "Staatliches", cursive;
  font-size: 20px;
  color: rgb(253, 236, 0);
}
.background {
  background-image: url(@/assets/Mac.jpg);
  background-size: cover;
  width: 100%;
  height: 120%;
  object-fit: cover;
  padding: 40px;
}
a {
  text-decoration: none;
}
img {
  display: block;
  margin-left: auto;
  margin-right: auto;
  margin-top: 15px;
  border-radius: 220px;
  border: 3px solid black;
}

#myPic {
  width: 200px;
  height: 200px;
  object-fit: cover;
  filter: sepia(var(--sepia, 0)) grayscale(var(--grrayscale, 0))
    invert(var(--invert, 0));
}

.filter {
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  position: relative;
  bottom: 12px;
}

.center {
  text-align: center;
  color: rgb(0, 0, 0);
  position: relative;
  bottom: 17px;
}

@media only screen and (max-width: 600px) {
  .filter {
    flex-direction: column;
    margin: 0 auto;
    align-items: center;
    gap: 8px;
  }
}
</style>
