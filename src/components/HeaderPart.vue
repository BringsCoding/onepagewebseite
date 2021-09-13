<template>
  <div class="maincontainer">
    <div class="thecard">
      <div class="thefront">
        <h1>Herzlich Wilkommen</h1>
        <p>*click me</p>
      </div>
      <div class="theback">
        <h3 class="rotate">Auf meiner Webseite</h3>
      </div>
    </div>
  </div>
</template>

<style scoped>
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

.maincontainer {
  position: relative;
  height: 150px;
  background-color: rgb(219, 219, 219);
}

p {
  font-size: 12px;
}
.thecard {
  position: absolute;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  transition: all 0.8s ease;
  background-color: blue;
}

.thecard:active {
  transform: rotateX(180deg);
}

.thefront {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  color: black;
  font-size: 25px;
  text-align: center;
  background: rgb(2, 0, 36);
  background: linear-gradient(
    331deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(73, 228, 17, 1) 0%,
    rgba(215, 86, 86, 1) 0%,
    rgba(227, 255, 104, 1) 100%,
    rgba(84, 93, 255, 1) 100%
  );
}

.theback {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  color: rgb(0, 0, 0);
  transform: rotateY(180deg);
  transform-style: preserve-3d;
  background-color: rgb(60, 199, 199);
  font-family: "Roboto", sans-serif;
}

.rotate {
  transform: rotate(180deg);
  font-size: 35px;
  text-align: center;
  margin-top: 50px;
  font-family: "Roboto", sans-serif;
}

@media only screen and (max-width: 461px) {
  p {
    position: relative;
    bottom: 180px;
  }
}
</style>
