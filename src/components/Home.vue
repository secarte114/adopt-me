<template>
  <div>
    <nav>
      <div class="logo-with-text">
        <img class="logo" src="../assets/img/logo.png" alt="AdoptMe.org Logo" />
        <h2>AdoptMe.org</h2>
      </div>
      <div id="nav-links">
        <a href="#">WHAT we do</a>
        <a href="#">WHO we are</a>
        <a href="#">EVENTS adoption</a>
      </div>
    </nav>
    <div class="hero">
      <div class="hero-text">
        <h1>This is your new Family</h1>
        <button>Adopt Now</button>
      </div>
    </div>

    <!-- MIDDLE IMAGES -->

    <b-container class="middle-container">
      <b-row>
        <b-col id="volunteer-container" cols="4" fluid="lg">
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
        <b-col id="testimonial-container" cols="7" fluid="xl">
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

    
    <b-container id="dog-vest-container">
      <b-row id="mid-links">
      <b-col cols="1" fluid="sm">PROGRAMS</b-col>
      <b-col cols="2" fluid="sm">ASSOCIATED COMPANIES</b-col>
    </b-row>
      <b-row>
        <b-col>
          <b-container class="programs">
            <b-row class="programs-container">
              <b-col cols="2"
                ><img src="../assets/img/friend-in-trouble.png" alt="Dog in a dog house" />
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
                ><img
                  src="../assets/img/dog-friends.png"
                  alt="Two friendly dogs"
              /></b-col>
              <b-col class="programs-text">
                <h4>MY NEXT FAMILY</h4>
                <p>
                  Are you looking for a new family member? The this program is
                  for you. Don't buy, adopt here, and let's give a home to these
                  amazing friends
                </p>
                <button class="read-more">READ MORE</button>
              </b-col>
            </b-row>
          </b-container>
        </b-col>
        <b-col cols="4"
          ><img id="dog-in-vest" src="../assets/img/dog-in-vest.png" alt="Dog in an adopt me vest"
        /></b-col>
      </b-row>
    </b-container>

    <!-- FOOTER -->
    <hr>
    <footer>
      <b-containter>
        <b-row>
          <b-col >
            <b-container>
              <b-row class="bottom-logo d-inline-flex" cols="4" >
                <img id="footer-logo" src="../assets/img/logo.png" alt="AdoptMe.org Logo" />
                <h1>AdoptMe.org</h1>
              </b-row>
              <b-row id="address">
                <p>Main St #1245</p>
                <p>Amazing City, 45677</p>
              </b-row>
            </b-container>
          </b-col>
          <b-col id="bottom-links" cols="8" align-v="center">
            <a href="#">WHAT we do</a>
            <a href="#">WHO we are</a>
            <a href="#">EVENTS adoption</a>
          </b-col>
        </b-row>

        <p id="upsplash">Some images were taken from upsplash.com</p>
      </b-containter>
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
  padding: 1rem 8rem;
  justify-content: space-between;
  align-items: center;
  font-family: $font-family-secondary;
}

.logo-with-text {
  display: flex;
  color: white;
  align-items: center;
}

#nav-links {
  display: flex;
  justify-content: space-between;
  font-weight: bolder;
  font-family: $font-family-primary;
  font-size: 1rem;
}

a {
  color: white !important;
  text-decoration: none !important;
  padding: 1rem;
}

.hero {
  background-image: url(../assets/img/dogs.jpg);
  height: 500px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
  vertical-align: bottom;
}

.hero-text {
  background: rgba(0, 0, 0, 0.2);
  position: absolute;
  bottom: -18%;
  left: 50%;
  transform: translate(-50%, -50%);
  width: 100%;
  color: $color-red;
  padding: 2% 10%;
  padding-left: 10%;
  margin-bottom: 0;
}

.hero-text h1 {
  font-family: $font-family-secondary;
  font-size: 60px;
  font-weight: 300;
}

.hero-text button {
  border: 2px $color-red solid;
  background-color: transparent;
  padding: 0.5% 2%;
  font-weight: bold;
  color: $color-red;
}

.middle-container {
  margin: 5% 8%;
  font-family: $font-family-secondary;
  font-size: 20px;
  font-weight: bold;
}

#volunteer-container {
  box-shadow: 2px 3px 10px rgb(0 0 0 / 0.2);
  padding: 0;
}

#volunteer-header {
  color: white;
  background-color: $color-blue;
  padding: 1rem;
  margin: 0px auto;
  font-family: $font-family-secondary;
  font-weight: bold;
}

#volunteer-container button {
  border: 2px $color-blue solid;
  background-color: white;
  padding: 1% 5%;
  font-weight: bolder;
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
  padding: 1rem;
  margin: 0px auto;
  font-family: $font-family-secondary;
  font-weight: bold;
}

#testimonial-container img {
  width: 100%;
}

#mid-links {
  display: flex;
  flex-direction: row;
  font-weight: bolder;
  margin-left: 1%;
  margin-bottom: 1rem;
  font-size: 1.4rem;
  font-family: $font-family-secondary;
}

#mid-links h2 {
  margin-left: 3%;
  margin-bottom: 2%;
}

#mid-links :hover {
  color: $color-blue !important;
  text-decoration: underline !important;
}

.programs-container {
  margin-left: 10%;
  margin-bottom: 2%;
  font-family: $font-family-secondary;
  font-weight: bold;
}

.programs-container img {
  width: 110%;
}

.programs-text {
  margin-bottom: 0;
  
}
.programs-container h4 {
  color: $color-red;
  font-weight: bold;
  font-family: $font-family-secondary;
}
.programs-container {
  color: $color-gray;
}

.programs-container button {
  border: 2px $color-red solid;
  background-color: white;
  padding: 1% 5%;
  font-weight: bold;
  color: $color-red;
  margin-bottom: 0;
}

#dog-in-vest {
  display: inline-block;
  width: 100%;
  vertical-align: middle;
}


.bottom-logo {
  color: white;
  justify-items: center !important;
}


#footer-logo{
  padding: 0;
}

footer {
  background-color: $color-blue;
  padding-top: 5%;
  padding-left: 10%;
  padding-bottom: 6%;
  color:white;
  align-items: center;
}

hr {
  border: .25rem solid $color-red !important;
  opacity: 1 !important;
  margin-bottom: 0 !important;
}

footer p{
  line-height: .5;
}

#address{
  padding-top: 5%;
}

#upsplash{
  background-color: $color-blue;
  color: white;
  padding-top: 2%;
  padding-bottom: 3%;
  padding-left: 1.5%;
  margin-bottom: 0;
}

#bottom-links{
  text-align: left;
  padding-left: 10%;
  font-weight: bold;
  font-size: large;
  font-family: $font-family-primary;
}
</style>