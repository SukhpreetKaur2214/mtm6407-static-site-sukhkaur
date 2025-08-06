<template>
  <section class="about-page container">
    <h1>About Me</h1>
    <div class="content">
      <p>
        Hi! I’m <strong>Sukhpreet</strong>, a passionate and driven student studying Web Development at Humber College.
        I have a strong interest in front-end technologies and design, and I enjoy building websites that are clean, responsive, and accessible.
      </p>
      <p>
        Outside of school, I love exploring UI/UX trends, learning new frameworks, and practicing what I learn through personal projects.
        I’m also interested in digital art and photography, which often inspires the aesthetics of my work.
      </p>
      <p>
        This website reflects my growth as a developer and includes real examples of the skills I’ve developed through hands-on learning.
      </p>
    </div>
  </section>
</template>

<style scoped>
.about-page {
  max-width: 900px;
  margin: 3rem auto;
  padding: 2rem 1.5rem;
  background-color: #121212;
  border-radius: 12px;
  box-shadow: 0 6px 18px rgba(0, 0, 0, 0.7);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #eee;
}

.about-page h1 {
  font-size: 2.4rem;
  margin-bottom: 1.5rem;
  color: #00bfa5;
  text-align: center;
}

.content p {
  line-height: 1.6;
  margin-bottom: 1.3rem;
  font-size: 1.1rem;
  color: #ccc;
}

.content strong {
  color: #00bfa5;
}

@media (max-width: 600px) {
  .about-page {
    margin: 2rem 1rem;
    padding: 1.5rem;
  }

  .about-page h1 {
    font-size: 2rem;
  }
}
</style>
