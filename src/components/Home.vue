
<template>
  <section id="home">
    <h1>Eniela Vela</h1>
    <p>Software Developer | Technical Writer | Tech Content Creator</p>
  </section>
</template>

<style scoped>
/* Home Section Styles */
#home {
  background: linear-gradient(to right, #2c3e50, #34495e);  /* Gradient background for emphasis */
  height: 100vh;  /* Full viewport height */
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #fff;  /* White text for contrast */
}

/* Animation for the main header */
@keyframes fadeInDown {
  0% {
    transform: translateY(-30px);
    opacity: 0;
  }
  100% {
    transform: translateY(0);
    opacity: 1;
  }
}

h1 {
  animation: fadeInDown 0.5s forwards;
  animation-delay: 0.3s;
  font-size: 3em;  /* Larger font size for emphasis */
  margin-bottom: 20px;
}

/* Animation for the subheader */
p {
  animation: fadeInUp 0.5s forwards;
  animation-delay: 0.5s;
  font-size: 1.2em;  /* Slightly larger font size for readability */
}

</style>
