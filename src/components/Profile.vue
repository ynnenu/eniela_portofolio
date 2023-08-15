
<template>
  <section id="profile" class="card">
    <h2>Profile</h2>
    <p><!-- Profile content goes here --></p>
  </section>
</template>

<style scoped>
/* Profile Section Styles */
#profile {
  background-image: url('path_to_your_image.jpg');  /* Placeholder - Replace with actual image path */
  background-size: cover;
  background-position: center;
  padding: 80px 20px;
  color: #fff;  /* White text to contrast with the background */
}

/* Animation for the header */
@keyframes slideInFromLeft {
  0% {
    transform: translateX(-100%);
    opacity: 0;
  }
  100% {
    transform: translateX(0);
    opacity: 1;
  }
}

h2 {
  animation: slideInFromLeft 0.5s forwards;
  animation-delay: 0.3s;
}

/* Animation for the content */
@keyframes fadeInUp {
  0% {
    transform: translateY(20px);
    opacity: 0;
  }
  100% {
    transform: translateY(0);
    opacity: 1;
  }
}

p {
  animation: fadeInUp 0.5s forwards;
  animation-delay: 0.5s;
}
</style>
