
<template>
  <section id="contact">
    <h2>Contact Me</h2>
    <form class="contact-form">
      <input type="text" placeholder="Your Name">
      <input type="email" placeholder="Your Email">
      <textarea rows="5" placeholder="Your Message"></textarea>
      <button type="submit">Send Message</button>
    </form>
  </section>
</template>
<script>
export default {
  name: "ContactMe",
}
</script>

<style scoped>
/* Contact Section Styles */
#contact {
  background-color: #2c3e50;  /* Neutral dark shade for emphasis */
  padding: 60px 20px;
  color: #fff;  /* White text for contrast */
}

.contact-form input, .contact-form textarea, .contact-form button {
  width: 100%;
  padding: 10px;
  margin-bottom: 20px;
  border: 2px solid #fff;  /* White border for contrast */
  background: transparent;
  color: #fff;  /* White text for contrast */
  transition: all 0.3s ease;  /* Transition for hover and focus effects */
}

.contact-form input:hover, .contact-form textarea:hover, .contact-form button:hover,
.contact-form input:focus, .contact-form textarea:focus {
  border-color: #f39c12;  /* A shade of orange for interactivity */
}

.contact-form button {
  cursor: pointer;
  text-align: center;
}

</style>

