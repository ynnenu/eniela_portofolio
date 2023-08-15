
<template>
  <div id="app">
    <Home />
    <Profile />
    <Employment />
    <ContactMe />
  </div>
</template>
<script>
import Home from './components/Home.vue'
import Profile from './components/Profile.vue'
import Employment from './components/Employment.vue'
export default {
  name: 'App',
  components: {
    Home,
    Profile,
    Employment
  }
}
</script>

<style>
/* Global Styles */
body {
  font-family: 'Arial', sans-serif;
  margin: 0;
  padding: 0;
  background-color: #f6f9fc;
  color: #333;
}

#app {
  max-width: 1200px;
  margin: 0 auto;
  padding: 20px;
  background-color: #fff;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
}

section {
  padding: 60px 0;
  text-align: center;
}

h1, h2 {
  color: #2c3e50;
}

h1 {
  font-size: 2.5em;
  margin-bottom: 10px;
}

h2 {
  font-size: 2em;
  margin-bottom: 20px;
}

p {
  font-size: 1em;
  line-height: 1.8;
  max-width: 800px;
  margin: 20px auto;
}

/* Contact Form Styles */
.contact-form {
  display: flex;
  flex-direction: column;
  max-width: 400px;
  margin: 0 auto;
}

.contact-form input, .contact-form textarea {
  padding: 10px;
  margin-bottom: 10px;
  border: 1px solid #e7e7e7;
  border-radius: 5px;
  font-size: 1em;
  width: 100%;
  transition: border-color 0.3s ease;
}

.contact-form input:focus, .contact-form textarea:focus {
  border-color: #2c3e50;
  outline: none;
}

.contact-form button {
  padding: 10px 15px;
  background-color: #2c3e50;
  color: #fff;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  transition: background-color 0.3s ease;
}

.contact-form button:hover {
  background-color: #34495e;
}

/* Responsive Design */
@media (max-width: 768px) {
  h1 {
    font-size: 2em;
  }

  h2 {
    font-size: 1.5em;
  }
}
</style>
