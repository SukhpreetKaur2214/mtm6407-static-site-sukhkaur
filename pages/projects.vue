<template>
  <div class="projects-page">
    <h1>My Projects</h1>
    <p class="intro">Below are some of the web development projects I've built to enhance my skills and explore modern tools and design techniques.</p>

    <div class="projects-list">
      <div class="project-card" v-for="project in projects" :key="project.title">
        <h2>{{ project.title }}</h2>
        <p>{{ project.description }}</p>
        <span class="tech">{{ project.tech }}</span>
      </div>
    </div>
  </div>
</template>

<script setup>
const projects = [
  {
    title: 'Responsive Portfolio Site',
    description: 'A fully responsive site built with Next.js and Tailwind CSS to showcase my personal and class projects.',
    tech: 'Next.js • Tailwind CSS',
  },
  {
    title: 'To-Do List App',
    description: 'A functional and minimal app created with vanilla JavaScript, allowing users to add, complete, and delete tasks.',
    tech: 'HTML • CSS • JavaScript',
  },
  {
    title: 'Contact Book (Vue.js)',
    description: 'Built during MTM6407, this app uses Vue 3, Vue Router, and local storage to manage contact information.',
    tech: 'Vue 3 • Vue Router • Local Storage',
  },
  {
    title: 'Photo Gallery Page',
    description: 'A grid-style image gallery using CSS Grid and JavaScript modals for full-size previews.',
    tech: 'CSS Grid • JavaScript',
  },
  {
    title: 'Static Site with Eleventy',
    description: 'My first attempt at a static site generator (before using Next.js), focused on learning templating and Markdown.',
    tech: 'Eleventy • Nunjucks • Markdown',
  },
]
</script>

<style scoped>
.projects-page {
  max-width: 1100px;
  margin: 3rem auto;
  padding: 2rem;
  background-color: #f9fafc;
  border-radius: 16px;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.06);
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  color: #222;
}

.projects-page h1 {
  font-size: 2.8rem;
  margin-bottom: 1rem;
  text-align: center;
  color: #1565c0;
  font-weight: bold;
}

.intro {
  text-align: center;
  font-size: 1.15rem;
  color: #444;
  max-width: 800px;
  margin: 0 auto 2rem;
}

.projects-list {
  display: grid;
  gap: 2rem;
  grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
}

.project-card {
  background-color: white;
  border-left: 6px solid #1565c0;
  padding: 1.5rem;
  border-radius: 10px;
  box-shadow: 0 6px 14px rgba(0, 0, 0, 0.04);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.project-card:hover {
  transform: translateY(-6px);
  box-shadow: 0 12px 30px rgba(0, 0, 0, 0.08);
}

.project-card h2 {
  font-size: 1.4rem;
  color: #0d47a1;
  margin-bottom: 0.5rem;
}

.project-card p {
  font-size: 1rem;
  color: #444;
  margin-bottom: 0.75rem;
}

.tech {
  display: inline-block;
  padding: 0.35rem 0.75rem;
  font-size: 0.85rem;
  background-color: #e3f2fd;
  color: #0d47a1;
  border-radius: 6px;
  font-weight: 600;
}
</style>
