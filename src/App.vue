<script>
import ServicesPage from "./components/ServicesPage.vue";
import FooterComponent from "./components/FooterComponent.vue";
import ContactComponent from "./components/ContactComponent.vue";

import './styles/base.css';
export default {
  name: 'App',
  components: {
    ServicesPage,
    FooterComponent,
    ContactComponent
  }
}
</script>

<template>
  <div class="logo-container d-flex justify-content-center align-items-center position-relative bg-white">
    <img src="@/assets/logo.png" alt="Elite Flooring Logo" class="logo p-1" />
  </div>
  <section id="app" class="v-100 d-flex justify-content-center align-items-center">
    <div class="intro text-center px-5 py-3 mb-5 ">
      <div class="logo-container d-flex justify-content-center align-items-center position-relative bg-white">
    <img src="@/assets/logo.png" alt="Elite Flooring Logo" class="logo-2 p-1" />
  </div>
 <p class="mt-2">Let us elevate your space</p>
 <a class="btn">Contact Us</a>
    </div>
</section>

 <section id="servicespage" class="about section p-4">
 <ServicesPage />
 </section>

 <section id="contact" class="section ">
  <ContactComponent/>
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
  height:90vh;
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
#contact{
    background-color: var(--dark-brown);
    border-top: 2px solid white;
        border-top: 2px solid white;
}
.section{
  height:100vh;
}
.intro{
background-color: rgb(255, 255, 255);
  border: 2px solid var(--medium-brown);
  border-radius: 5px;

}
/* Logo Section */
.logo-container {

height: 10vh;
}

.logo {
  width: 250px;
  height: 70px;
  object-fit: contain; /* Ensure proper scaling */
}
.logo-2 {
  width: 250px;
  height: 90px;
  object-fit: contain; /* Ensure proper scaling */
}
.btn{
  background-color: var(--medium-brown);
  color:white;
  border: 2px solid white;
}
.btn:hover{
  background-color: var(--dark-brown);
}
.header {
  font-family: 'CustomFont1', serif;
 color: var(--dark-brown)
}
</style>
