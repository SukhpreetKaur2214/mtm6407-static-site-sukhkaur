<template>
    <div>
      <h1>Blog</h1>
      <p>Web development allows me to mix creativity with problem-solving, and that’s what excites me most about it.

I started by learning basic HTML and CSS, but once I built my first interactive website using JavaScript, I was hooked. Since then, I’ve explored tools like React, Tailwind, Vue, and now Next.js.

Through this blog, I want to share insights from my learning journey—like tips for responsive design, fun CSS tricks, and reflections on the challenges of building full websites as a student. The more I build, the more confident I feel in my abilities, and I’m excited to keep growing.

</p>
    </div>
  </template>
  <style scoped>
.blog-page {
  max-width: 900px;
  margin: 3rem auto;
  padding: 2rem 1.5rem;
  background-color: #004d40; /* dark teal */
  border-radius: 12px;
  box-shadow: 0 6px 18px rgba(0, 77, 64, 0.6);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #e0f2f1; /* light teal */
  line-height: 1.6;
}

.blog-page h1 {
  font-size: 2.6rem;
  margin-bottom: 1.5rem;
  color: #00bfa5; /* bright teal accent */
  text-align: center;
}

.blog-page p {
  font-size: 1.1rem;
  margin-bottom: 1.4rem;
  color: #b2dfdb;
}

@media (max-width: 600px) {
  .blog-page {
    margin: 2rem 1rem;
    padding: 1.5rem 1rem;
  }

  .blog-page h1 {
    font-size: 2rem;
  }
}
</style>
