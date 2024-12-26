<template>
    <footer class="footer-container">
      <!-- Left Section: Social Media Icons -->
      <div class="social-icons">
        <a href="https://github.com/betocv13" target="_blank" rel="noopener noreferrer">
          <img src="@/assets/mail.png" alt="GitHub" class="footer-icon" />
        </a>
        <a href="https://linkedin.com/in/betocv13" target="_blank" rel="noopener noreferrer">
          <img src="@/assets/phone.png" alt="LinkedIn" class="footer-icon" />
        </a>
      </div>
  
      <!-- Right Section: Copyright Text -->
      <div class="copyright-text">
        © 2024 EliteFlooring LLC. All Rights Reserved.
      </div>
    </footer>
  </template>
  
  <script>
  export default {
    name: "FooterComponent",
  };
  </script>
  
  <style scoped>
 .footer-container {
  position: relative; /* Required for z-index to work */
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: var(--medium-brown); /* Background color for footer */
  color: #fff; /* Text color */
  padding: 20px 20px; /* Padding around the footer */
  font-size: 0.9rem; /* Adjust font size for copyright text */
  z-index: 10000; /* Ensures it is above other elements */
}

  .social-icons {
    display: flex;
    gap: 10px; /* Spacing between the icons */
  }
  
  .footer-icon {
    width: 25px; /* Adjust size of the icons */
    height: 25px;
    object-fit: contain;
    cursor: pointer;
    transition: transform 0.3s ease; /* Add hover effect */
  }
  
  .footer-icon:hover {
    transform: scale(1.1); /* Slight zoom effect on hover */
  }
  
  .copyright-text {
    text-align: right;
    font-size: 0.8rem; /* Slightly smaller font for copyright text */
  }

@media (max-width: 767px) {
    .copyright-text {
    text-align: right;
    font-size: 0.7rem; /* Slightly smaller font for copyright text */
  }
}
  </style>
  