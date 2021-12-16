<template>
  <div>
    <nav>
      <img src="../assets/img/logo.png" alt="AdoptMe.org Logo" />
      <h1>AdoptMe.org</h1>
      <a href="#">WHAT we do</a>
      <a href="#">WHO we are</a>
      <a href="#">EVENTS adoption</a>
    </nav>
    <section class="hero-banner">
      <h1>This is your new Family</h1>
      <button>Adopt Now</button>
    </section>
    <section>
      <h2>Volunteers</h2>
      <img src="../assets/img/girl.png" alt="Girl carrying dog">
      <p>Amazing people, doing the difference evrey single day. Join us know and be a part of a community that is changing the world</p>
      <button>Join Us</button>
    </section>
    <section>
      <h2>Testimonial of the Month</h2>
      <img src="../assets/img/testimonial.jpg" alt="testimonial video">
    </section>
    <footer>
       <img src="../assets/img/logo.png" alt="AdoptMe.org Logo" />
      <h1>AdoptMe.org</h1>
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

h1 {
  color: white;
}

a {
  color: white;
  text-decoration: none;
}

#hero-banner{
    position:relative;
    padding:1rem;
    grid-area:center-panel;
    display:flex;
    flex-direction: column;
    justify-content: center;
  }

.hero-banner::before{
    background-image: url('../assets/img/dogs.jpg');
    height: 2rem;  
    background-position: center; 
    background-repeat: no-repeat; 
    background-size: cover;
    opacity:0.5;
    position:absolute;
    top:0;
    bottom:0;
    right:0;
    left:0;
    width:auto;
    height:auto;
    z-index:-3;
}

footer{
  background-color: $color-blue;
}
</style>