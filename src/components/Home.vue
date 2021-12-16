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
    <div class="middle-container">
      <div id="volunteer-container">
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
        <button>Join Us</button>
      </div>
      <div id="testimonial-container">
        <h2 id="testimonial-header">TESTIMONIAL OF THE MONTH</h2>
        <img
          id="testimonial-image"
          src="../assets/img/testimonial.jpg"
          alt="testimonial video"
        />
      </div>
    </div>
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
  opacity: .3;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  
}

.hero-text h1 {
  color: $color-blue;
  opacity: 100%;
}

.middle-container {
  display: grid;
  grid-template-columns: 1fr 1fr;
  grid-template-areas: "volunteer testimonial";
  grid-gap: 4%;
  margin: 5% 8%;
}

.volunteer-container {
  grid-area: volunteer;
  border: 1px solid black;
}

#volunteer-header {
  color: white;
  background-color: $color-blue;
  padding: 0.5rem;
  margin: 0px auto;
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

footer {
  background-color: $color-blue;
}
</style>