
<template>
  <section id="profile" class="card">
    <h2>Profile</h2>
    <p>
<svg width="200px" height="100px" viewBox="0 0 200 100" xmlns="http://www.w3.org/2000/svg">
    <!-- Cloud shape -->
    <path d="M50 80 Q 40 60 50 40 Q 70 20 90 40 Q 110 60 130 40 Q 150 20 170 40 Q 180 60 170 80 Z" fill="white"/>
</svg>
</p>
  </section>
</template>

<style scoped>
/* Profile Section Styles */
#profile {
    /* Placeholder - Replace with actual image path */
  
  
  padding: 80px 20px;
  color: #fff; background-color: black;  /* White text to contrast with the background */
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

<style>
    @keyframes moveCloud {
        0% {
            transform: translateX(-100%);
        }
        100% {
            transform: translateX(100%);
        }
    }

    .cloud-container {
        width: 200px;
        height: 100px;
        background-color: black;
        overflow: hidden;
    }

    .moving-cloud {
        animation: moveCloud 30s linear infinite;
    }
</style>

<!-- Cloud with animation inside a container -->
<div class="cloud-container">
    <svg class="moving-cloud" width="200px" height="100px" viewBox="0 0 200 100" xmlns="http://www.w3.org/2000/svg">
        <!-- Cloud shape -->
        <path d="M50 80 Q 40 60 50 40 Q 70 20 90 40 Q 110 60 130 40 Q 150 20 170 40 Q 180 60 170 80 Z" fill="white"/>
    </svg>
</div>

<style>
    .clouds-container {
        position: relative;
        width: 100%;
        height: 100%;
        overflow: hidden;
    }

    .cloud1, .cloud2, .cloud3 {
        position: absolute;
        bottom: 0;
        animation-duration: 60s;
        animation-timing-function: linear;
        animation-iteration-count: infinite;
    }

    .cloud1 {
        animation-name: moveCloud1;
        left: 0;
    }

    .cloud2 {
        animation-name: moveCloud2;
        right: 0;
    }

    .cloud3 {
        animation-name: moveCloud3;
        left: 50%;
        transform: translateX(-50%);
    }

    @keyframes moveCloud1 {
        0% { transform: translateX(-100%); }
        100% { transform: translateX(100%); }
    }

    @keyframes moveCloud2 {
        0% { transform: translateX(100%); }
        100% { transform: translateX(-100%); }
    }

    @keyframes moveCloud3 {
        0% { transform: translateX(-50%) translateY(0); }
        100% { transform: translateX(-50%) translateY(-10%); }
    }
</style>
