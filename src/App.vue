<script>
import ServicesPage from "./components/ServicesPage.vue";
import FooterComponent from "./components/FooterComponent.vue";
import './styles/base.css';
export default {
  name: 'App',
  components: {
    ServicesPage,
    FooterComponent
  }
}
</script>

<template>
  <section id="app" class="v-100 d-flex justify-content-center align-items-center">
    <div class="intro text-center px-5 py-3 mb-5 ">
 <h1 class="header align-items-center display-3 text-white fs-bold fw-bold ">Elite Flooring</h1>
 <p>Let us elevate your space</p>
 <a class="btn">Contact Us</a>
    </div>
  
</section>

 <section id="servicespage" class="about section p-4">
 <ServicesPage />
 </section>

 <section id="contact" class="section bg-primary">
  <h1>contact</h1>
</section>

<section id="footer" class="">
    <FooterComponent />
    </section>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;

  color: #000000;
  background-image: url('@/assets/pic1.jpg');
  background-size: cover;
  background-position: center;
  height:100vh;
}
#servicespage {
  position: relative;
  background-image: url('@/assets/pic3.jpg');
  background-size: cover;
  background-position: center;
  height: 100vh;
  color: white;
  overflow: hidden; /* Ensures no overflow from child elements */
}

#servicespage::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(43, 37, 33, 0.8); /* Semi-transparent overlay */
  z-index: 1; /* Ensures it sits above the background image */
}

#servicespage > * {
  position: relative;
  z-index: 2; /* Ensures content sits above the overlay */
}
.section{
  height:100vh;
}
.intro{
  background-color: var(--brown-opacity);
  border: 2px solid var(--medium-brown);
  border-radius: 5px;

}
.about{

}
.btn{
  background-color: var(--medium-brown);
  color:white;
  border: 2px solid white;
}
.btn:hover{
  background-color: var(--dark-brown);
}
</style>
