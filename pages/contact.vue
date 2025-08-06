<template>
  <div class="contacts-page">
    <h1>Get in Touch</h1>
    <p class="intro">
      Thanks for visiting! Whether you're a fellow student, teacher, or collaborator, feel free to reach out.
      I'm always open to networking, feedback, and new opportunities.
    </p>

    <div class="contact-list">
      <div class="contact-item">
        <span aria-label="Email" role="img">📧</span>
        <strong>Email:</strong>
        <a href="mailto:sukhpreet.dev@example.com">sukhpreet.dev@example.com</a>
      </div>

      <div class="contact-item">
        <span aria-label="GitHub" role="img">💼</span>
        <strong>GitHub:</strong>
        <a href="https://github.com/sukhpreet" target="_blank" rel="noopener">github.com/sukhpreet</a>
      </div>

      <div class="contact-item">
        <span aria-label="Instagram" role="img">📷</span>
        <strong>Instagram:</strong>
        <a href="https://instagram.com/sukh.design" target="_blank" rel="noopener">@sukh.design</a>
      </div>

      <div class="contact-item">
        <span aria-label="Location" role="img">📍</span>
        <strong>Location:</strong>
        <span>Toronto, ON</span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.contacts-page {
  max-width: 850px;
  margin: 3rem auto;
  padding: 2rem 2.5rem;
  background-color: #111;
  color: #e0f2f1;
  border-radius: 16px;
  box-shadow: 0 10px 30px rgba(0, 0, 0, 0.75);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.contacts-page h1 {
  text-align: center;
  font-size: 2.8rem;
  color: #64ffda;
  font-weight: 700;
  margin-bottom: 1rem;
}

.intro {
  text-align: center;
  font-size: 1.2rem;
  color: #b2dfdb;
  margin-bottom: 2.5rem;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}

.contact-list {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.contact-item {
  background-color: #1b1b1b;
  padding: 1.25rem 1.5rem;
  border-left: 5px solid #64ffda;
  border-radius: 12px;
  box-shadow: 0 6px 20px rgba(0, 0, 0, 0.4);
  display: flex;
  align-items: center;
  gap: 1rem;
  font-size: 1.05rem;
  transition: transform 0.3s ease;
}

.contact-item:hover {
  transform: scale(1.02);
}

.contact-item span[role="img"] {
  font-size: 1.4rem;
}

.contact-item strong {
  color: #81c784;
  min-width: 90px;
  flex-shrink: 0;
}

.contact-item a {
  color: #80cbc4;
  text-decoration: none;
  word-break: break-word;
}

.contact-item a:hover {
  text-decoration: underline;
}

@media (max-width: 600px) {
  .contacts-page {
    margin: 2rem 1rem;
    padding: 1.5rem;
  }

  .contacts-page h1 {
    font-size: 2rem;
  }

  .contact-item {
    flex-direction: column;
    align-items: flex-start;
  }

  .contact-item strong {
    margin-bottom: 0.3rem;
  }
}
</style>
