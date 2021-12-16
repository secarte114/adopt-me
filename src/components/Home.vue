<template>
  <div>
    <nav>
      <div class="logo-with-text">
        <img class="logo" src="../assets/img/logo.png" alt="AdoptMe.org Logo" />
        <h2>AdoptMe.org</h2>
      </div>
      <a href="#">WHAT we do</a>
      <a href="#">WHO we are</a>
      <a href="#">EVENTS adoption</a>
    </nav>
    <div class="hero-image">
      <div class="hero-text">
        <h1>This is your new Family</h1>
        <button>Adopt Now</button>
      </div>
    </div>

    <!-- MIDDLE IMAGES -->

    <b-container class="middle-container">
      <b-row>
        <b-col id="volunteer-container" cols="4">
          <h2 id="volunteer-header">VOLUNTEERS</h2>
          <img
            id="volunteer-image"
            src="../assets/img/girl.png"
            alt="Girl carrying dog"
          />
          <p>
            Amazing people, doing the difference evrey single day. Join us know
            and be a part of a community that is changing the world
          </p>
          <button>JOIN US</button>
        </b-col>
        <b-col id="testimonial-container" cols="8">
          <h2 id="testimonial-header">TESTIMONIAL OF THE MONTH</h2>
          <img
            id="testimonial-image"
            src="../assets/img/testimonial.jpg"
            alt="testimonial video"
          />
        </b-col>
      </b-row>
    </b-container>
    <!-- PROGRAMS -->

    <div id="mid-links">
      <h2>PROGRAMS</h2>
      <h2>ASSOCIATED COMPANIES</h2>
    </div>
    <b-container id="dog-vest-container">
      <b-row>
      <b-col>
        <b-container class="programs">
          <b-row class="programs-container">
            <b-col cols="2"
              ><img src="../assets/img/friend-in-trouble.png" alt="" />
            </b-col>
            <b-col class="programs-text">
              <h4>BEHAVIOR PROGRAM</h4>
              <p>
                Evaluation of each dog using specialist who determine the best
                training that will help your friend be a better family member
              </p>
              <button class="read-more">READ MORE</button>
            </b-col>
          </b-row>
          <b-row class="programs-container">
            <b-col cols="2"
              ><img src="../assets/img/dog-friends.png" alt="Two friendly dogs"
            /></b-col>
            <b-col class="programs-text">
              <h4>MY NEXT FAMILY</h4>
              <p>
                Are you looking for a new family member? The this program is for
                you. Don't buy, adopt here, and let's give a home to these
                amazing friends
              </p>
              <button class="read-more">READ MORE</button>
            </b-col>
          </b-row>
        </b-container>
      </b-col>
      <b-col cols="4"
        ><img id="dog-in-vest" src="../assets/img/dog-in-vest.png" alt=""
      /></b-col>
      </b-row>
    </b-container>

    <!-- FOOTER -->
    <footer>
      <div class="logo-with-text">
        <img src="../assets/img/logo.png" alt="AdoptMe.org Logo" />
        <h1>AdoptMe.org</h1>
      </div>
      <a href="#">WHAT we do</a>
      <a href="#">WHO we are</a>
      <a href="#">EVENTS adoption</a>
    </footer>
  </div>
</template>

<script>
export default {
  name: "home",
};
</script>

<style lang="scss">
nav {
  background-color: $color-red;
  display: flex;
  margin: 0px;
  padding: 1rem;
  justify-content: space-evenly;
  align-items: center;
}

.logo-with-text {
  display: flex;
  color: white;
}

a {
  color: white;
  text-decoration: none;
}

.hero-image {
  background-image: url(../assets/img/dogs.jpg);
  height: 500px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  display: flex;
  flex-flow: column;
  justify-content: left;
}

.hero-text {
  background-color: black;
  opacity: 0.3;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  vertical-align: text-bottom;
  color: $color-red;
}

.hero-text button {
  border: 2px $color-red solid;
  background-color: transparent;
  padding: 0 1%;
  font-weight: bold;
  margin-left: 5%;
  color: $color-red;
}

.middle-container {
  margin: 5% 8%;
}

#volunteer-container {
  box-shadow: 2px 3px 10px rgb(0 0 0 / 0.2);
  padding: 0;
}

#volunteer-header {
  color: white;
  background-color: $color-blue;
  padding: 0.5rem;
  margin: 0px auto;
}

#volunteer-container button {
  border: 2px $color-blue solid;
  background-color: white;
  padding: 1% 5%;
  font-weight: bold;
  color: $color-blue;
  margin-left: 5%;
}

#volunteer-container p {
  color: $color-gray;
  padding: 5% 27%;
  padding-left: 5%;
  font-size: x-large;
}

#volunteer-image {
  width: 100%;
}
.testimonial-container {
  grid-area: testimonial;
}

#testimonial-header {
  color: white;
  background-color: $color-red;
  padding: 0.5rem;
  margin: 0px auto;
}

#testimonial-container img {
  width: 100%;
}

#mid-links {
  display: flex;
  flex-direction: row;
  font-weight: bolder;
  margin-left: 6%;
}

#mid-links h2 {
  margin-right: 5%;
}

#mid-links h2:hover {
  color: $color-blue;
  text-decoration: underline;
}

// .programs-container {
//   margin-left: 10%;
//   margin-bottom: 2%;
// }

.programs-container img {
  width: 100%;
}

.programs-container h4 {
  color: $color-red;
  font-weight: bold;
}
.programs-container p {
  color: $color-gray;
}

.programs-container button {
  border: 2px $color-red solid;
  background-color: white;
  padding: 1% 5%;
  font-weight: bold;
  color: $color-red;
}

// .programs-container{
//   display: flex;
//   flex-direction: row;
// }

#dog-in-vest {
  display: inline-block;
  width: 100%;
 vertical-align: middle;
}
footer {
  background-color: $color-blue;
  display: flex;
}
</style>