<script>
import '../styles/base.css';
export default {
  name: 'ContactComponent',
};
</script>

<template>
      <h1 class="header display-1 text-white px-2">Contact</h1>
   <div class="d-flex vh-100 justify-content-center align-items-center p-4">
  <div class="contact-form container p-4 rounded align-items-center justify-content-center">
    <h1 class="text-center mb-4">Contact Us</h1>
    <form class="row g-3">
      <!-- Name Input -->
      <div class="col-md-12">
        <label for="name" class="form-label">Name</label>
        <input
          type="text"
          id="name"
          class="form-control"
          placeholder="Enter your full name"
        />
      </div>

      <!-- Email Input -->
      <div class="col-md-12">
        <label for="email" class="form-label">Email</label>
        <input
          type="email"
          id="email"
          class="form-control"
          placeholder="example@gmail.com"
        />
      </div>

      <!-- Phone Input -->
      <div class="col-md-12">
        <label for="phone" class="form-label">Phone</label>
        <input
          type="tel"
          id="phone"
          class="form-control"
          placeholder="(515) 000-0000"
        />
      </div>

       <!-- Phone Input -->
       <div class="col-md-12">
        <label for="description" class="form-label">Description</label>
        <input
          type=""
          id="description"
          class="form-control"
          placeholder="brief description on for your project"
        />
      </div>

      <!-- Submit Button -->
      <div class="col-12 text-center mt-4">
        <button type="submit" class="btn px-4">Submit</button>
      </div>
    </form>
  </div>
</div>
</template>

<style>
.contact-form {
  background-color: var(--brown-opacity); /* Dark background for contrast */
  color: white;
  max-width: 600px; /* Restrict the form's width */
  margin: 0 auto; /* Center the form */
  border: 3px solid white;

}

.contact-form label {
  font-weight: bold; /* Make labels more prominent */
}
.btn{
  background-color: var(--medium-brown);
}

</style>