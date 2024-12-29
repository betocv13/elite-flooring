<script>
import '../styles/base.css';
export default {
  name: 'ServicesPage',
}
</script>

<template>
    <h1>SERVICES</h1>
    <hr class="line">
    <br>
    <p class="custom-font-size text-right">At <b>Elite Floors</b>, we pride ourselves on delivering top-quality flooring solutions to elevate your space. With years of experience and a commitment to excellence, we provide a range of flooring services to meet your needs. Whether you’re enhancing your home, upgrading a commercial space, or outfitting a specialized area, we’ve got you covered.</p>
    <br>

    <div class="services-list fs-5 fw-bold">
    <!-- Mobile Layout -->
    <div class="mobile-layout gap-0 d-md-none">
      <p>Floor Installation</p>
      <hr>
      <p>Gym Flooring</p>
      <hr>
      <p>LVT (Luxury Vinyl Tile) Flooring</p>
      <hr>
      <p>Laminate Flooring</p>
      <hr>
      <p>Floor Repairs</p>
      <hr>
      <p>And much more...</p>
    </div>

    <!-- Desktop Layout -->
    <ul class="desktop-layout d-none d-md-flex flex-column gap-4">
      <li>Floor Installation</li>
      <li>Hardwood Flooring</li>
      <li>Gym Flooring</li>
      <li>LVT (Luxury Vinyl Tile) Flooring</li>
      <li>Laminate Flooring</li>
      <li>Floor Repairs</li>
      <li>And much more...</li>
    </ul>
  </div>
</template>

<style>
   h1 {
  font-family: 'CustomFont1', serif;

}
#ServicesPage {
  background-image: url('@/assets/pic1.jpg');
  background-size: cover;
  background-position: center;
  height:100vh;
}

.custom-font-size {
  font-size: 1rem; 
}

@media (min-width: 576px) {
  .custom-font-size {
    font-size: 1.2rem;
  }
}

@media (min-width: 768px) {
  .custom-font-size {
    font-size: 1.5rem;
  }
}
</style>
