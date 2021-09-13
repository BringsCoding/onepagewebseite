<template>
  <div class="block">
    <div class="maincontainer">
      <div class="thecard">
        <div class="thefront">
          <h1>Infos über mich 🚨</h1>
        </div>
        <div class="theback">
          <p class="rotate">
            25 Jahre jung und Programmiere seit 10/2020.<br />
            Ich habe erfahrung in
            <span class="html-text">HTML(semantisch)</span><br />
            <span class="css-text">CSS(responsiv)</span><br />
            <span class="javascript-text">JavaScript</span><br />
            <span class="vue-text">Vue</span><br />
            <span class="node-text">NodeJs</span><br />
            <span class="github-text">GitHube/GitBash</span><br />
            <span class="cypress-text">Cypress und NPM</span>
          </p>
        </div>
      </div>
    </div>
    <div class="maincontainer-tow">
      <div class="thecard-tow">
        <div class="thefront-tow">
          <h1>Mein Weg <br />👨‍💻 💻</h1>
        </div>
        <div class="theback-tow">
          <p class="rotate-tow">
            Im Jahr 2021 beschloss ich das Bootcamp Europe zu besuchen, und
            meine vorhandenen Programmierfähigkeiten<br />
            noch weiter auszubauen.
          </p>
        </div>
      </div>
    </div>
    <div class="maincontainer-three">
      <div class="thecard-three">
        <div class="thefront-three">
          <h1>Mein Ziel</h1>
        </div>
        <div class="theback-three">
          <p class="rotate-three">
            In ein Unternehmen zu kommen, wo ich meine vorhandenen Fähigkeiten
            noch weiter ausbauen kann, und dazu lerne.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto&display=swap");
@import url("https://fonts.googleapis.com/css2?family=IBM+Plex+Sans:ital,wght@1,200&family=Roboto&display=swap");

/* Allgmein Block one */
*,
*::before,
*::after {
  box-sizing: border-box;
  font-family: "Roboto", sans-serif;
}
body {
  margin: 0;
}

.html-text {
  color: orange;
  font-family: "IBM Plex Sans", sans-serif;
  font-family: "Roboto", sans-serif;
}
.css-text {
  color: blue;
  font-family: "IBM Plex Sans", sans-serif;
  font-family: "Roboto", sans-serif;
}
.javascript-text {
  color: yellow;
  font-family: "IBM Plex Sans", sans-serif;
  font-family: "Roboto", sans-serif;
}
.vue-text {
  color: green;
  font-family: "IBM Plex Sans", sans-serif;
  font-family: "Roboto", sans-serif;
}
.github-text {
  color: rgb(182, 179, 179);
  font-family: "IBM Plex Sans", sans-serif;
  font-family: "Roboto", sans-serif;
}

.node-text {
  color: aquamarine;
  font-family: "IBM Plex Sans", sans-serif;
  font-family: "Roboto", sans-serif;
}
.block {
  display: flex;
  padding: 0.625rem;
  justify-content: space-around;
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

.maincontainer {
  position: relative;
  height: 450px;
  width: 350px;
  background-color: rgb(219, 219, 219);
}

.thecard {
  position: absolute;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  transition: all 0.8s cubic-bezier(0.4, 0, 1, 1);
  background-color: blue;
}

.thecard:hover {
  transform: rotateY(180deg);
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
    34deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(88, 88, 255, 1) 0%,
    rgba(80, 99, 255, 1) 0%,
    rgba(0, 212, 255, 1) 51%,
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
  background: rgb(2, 0, 36);
  background: linear-gradient(
    34deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(88, 88, 255, 1) 0%,
    rgba(80, 99, 255, 1) 0%,
    rgba(139, 3, 255, 1) 57%,
    rgba(84, 93, 255, 1) 100%
  );
}

.rotate {
  font-size: 25px;
  text-align: center;
  margin-top: 50px;
  font-family: "Roboto", sans-serif;
  color: azure;
}

/* Block-tow!! */

.maincontainer-tow {
  position: relative;
  height: 450px;
  width: 350px;
  background-color: rgb(219, 219, 219);
}

.thecard-tow {
  position: absolute;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  transition: all 0.8s cubic-bezier(0.4, 0, 1, 1);
  background-color: blue;
}

.thecard-tow:hover {
  transform: rotateY(180deg);
}

.thefront-tow {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  color: black;
  font-size: 25px;
  text-align: center;
  background: rgb(2, 0, 36);
  background: linear-gradient(
    34deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(88, 88, 255, 1) 0%,
    rgba(80, 99, 255, 1) 0%,
    rgba(0, 212, 255, 1) 51%,
    rgba(84, 93, 255, 1) 100%
  );
}

.theback-tow {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  color: rgb(0, 0, 0);
  transform: rotateY(180deg);
  transform-style: preserve-3d;
  background: rgb(2, 0, 36);
  background: linear-gradient(
    34deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(88, 88, 255, 1) 0%,
    rgba(80, 99, 255, 1) 0%,
    rgba(139, 3, 255, 1) 57%,
    rgba(84, 93, 255, 1) 100%
  );
}

.rotate-tow {
  font-size: 25px;
  text-align: center;
  margin-top: 50px;
  font-family: "Roboto", sans-serif;
  color: azure;
}

/* Block-threes!! */
.maincontainer-three {
  position: relative;
  height: 450px;
  width: 350px;
  background-color: rgb(219, 219, 219);
}

.thecard-three {
  position: absolute;
  width: 100%;
  height: 100%;
  transform-style: preserve-3d;
  transition: all 0.8s cubic-bezier(0.4, 0, 1, 1);
  background-color: blue;
}

.thecard-three:hover {
  transform: rotateY(180deg);
}

.thefront-three {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  color: black;
  font-size: 25px;
  text-align: center;
  background: rgb(2, 0, 36);
  background: linear-gradient(
    34deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(88, 88, 255, 1) 0%,
    rgba(80, 99, 255, 1) 0%,
    rgba(0, 212, 255, 1) 51%,
    rgba(84, 93, 255, 1) 100%
  );
}

.theback-three {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  color: rgb(0, 0, 0);
  transform: rotateY(180deg);
  transform-style: preserve-3d;
  background: rgb(2, 0, 36);
  background: linear-gradient(
    34deg,
    rgba(2, 0, 36, 1) 0%,
    rgba(88, 88, 255, 1) 0%,
    rgba(80, 99, 255, 1) 0%,
    rgba(139, 3, 255, 1) 57%,
    rgba(84, 93, 255, 1) 100%
  );
}

.rotate-three {
  font-size: 25px;
  text-align: center;
  font-family: "Roboto", sans-serif;
  color: azure;
  padding-bottom: 150px;
}

@media only screen and (max-width: 1000px) {
  .block {
    flex-direction: column;
    margin: 0 auto;
    align-items: center;
    gap: 8px;
    background-color: aquamarine;
  }
}
</style>
