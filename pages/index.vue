<template>
  <div class="home-page">
    <h1>Welcome to My Portfolio</h1>
    <p>
      Welcome to my portfolio site! My name is Sukhpreet, and I’m a web development student at Algonquin College.

      I created this site as part of my MTM6407 Web Development IV course using Next.js, a powerful React-based framework.

      This website showcases who I am, what I’ve built, and what I’ve learned. You can explore my current and past projects,

      read blog posts about my web development journey, and learn how to get in touch with me. Thank you for stopping by!
    </p>
  </div>
</template>

<style scoped>
.home-page {
  max-width: 880px;
  margin: 3rem auto;
  padding: 3rem 2rem;
  background: rgba(255, 255, 255, 0.15);
  backdrop-filter: blur(12px);
  border-radius: 18px;
  box-shadow: 0 12px 40px rgba(0, 0, 0, 0.2);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #222;
  animation: fadeIn 1s ease;
  background-image: linear-gradient(to bottom right, #e0f7fa, #ffffff);
  border: 1px solid rgba(255, 255, 255, 0.3);
  transition: transform 0.3s ease;
}

.home-page:hover {
  transform: scale(1.01);
}

.home-page h1 {
  font-size: 2.75rem;
  margin-bottom: 1.8rem;
  text-align: center;
  color: #0288d1;
  font-weight: 800;
  letter-spacing: 1px;
}

.home-page p {
  font-size: 1.2rem;
  color: #333;
  line-height: 1.75;
  text-align: justify;
  white-space: pre-line;
}

/* Animation */
@keyframes fadeIn {
  from {
    opacity: 0;
    transform: translateY(25px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Responsive Design */
@media (max-width: 600px) {
  .home-page {
    margin: 2rem 1rem;
    padding: 2rem 1.5rem;
  }

  .home-page h1 {
    font-size: 2.2rem;
  }

  .home-page p {
    font-size: 1.05rem;
  }
}
</style>

