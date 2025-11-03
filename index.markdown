---
layout: default
---

<div class="hero-section">
  <div class="hero-content">
    <h1 class="hero-title">Hi, I'm Saji Shunnarah 👋</h1>
    <p class="hero-subtitle">Passionate Software Engineer | M.S. Student @ Georgia Tech</p>
    <p class="hero-description">I craft innovative solutions and build scalable applications that make a difference</p>
    <div class="hero-cta">
      <a href="#projects" class="btn btn-primary">View My Work</a>
      <a href="#contact" class="btn btn-secondary">Get In Touch</a>
    </div>
  </div>
</div>

<section id="about" class="section">
  <div class="container">
    <h2 class="section-title">About Me</h2>
    <div class="about-content">
      <p>I'm an awarded software engineer with a passion for creating elegant solutions to complex problems. With expertise in full-stack development, I specialize in building scalable web applications using modern technologies.</p>
      <p>My approach combines technical excellence with user-centered design, ensuring that every project not only works flawlessly but also provides an exceptional user experience.</p>
      <p>I'm currently pursuing a Master's degree in Computer Science at Georgia Tech, deepening my expertise in advanced software engineering and human-computer interaction.</p>
    </div>
  </div>
</section>

<section id="skills" class="section section-alt">
  <div class="container">
    <h2 class="section-title">Technical Skills</h2>
    <div class="skills-grid">
      <div class="skill-category">
        <h3>Frontend</h3>
        <ul class="skill-list">
          <li>Angular</li>
          <li>React</li>
          <li>TypeScript</li>
          <li>HTML/CSS</li>
          <li>PrimeNG</li>
        </ul>
      </div>
      <div class="skill-category">
        <h3>Backend</h3>
        <ul class="skill-list">
          <li>Java SpringBoot</li>
          <li>Node.js</li>
          <li>RESTful APIs</li>
          <li>Microservices</li>
        </ul>
      </div>
      <div class="skill-category">
        <h3>Database & Cloud</h3>
        <ul class="skill-list">
          <li>PostgreSQL</li>
          <li>SupaBase</li>
          <li>Google Cloud Platform</li>
          <li>Cloud Hosting</li>
        </ul>
      </div>
      <div class="skill-category">
        <h3>Tools & Practices</h3>
        <ul class="skill-list">
          <li>Git & GitHub</li>
          <li>CI/CD</li>
          <li>Agile/Scrum</li>
          <li>JWT Authentication</li>
        </ul>
      </div>
    </div>
  </div>
</section>

<section id="projects" class="section">
  <div class="container">
    <h2 class="section-title">Featured Projects</h2>
    <div class="projects-grid">
      {% for post in site.posts %}
      <article class="project-card">
        <h3 class="project-title">
          <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
        </h3>
        <p class="project-date">{{ post.date | date: "%B %Y" }}</p>
        <div class="project-excerpt">
          {{ post.excerpt }}
        </div>
        <a href="{{ post.url | relative_url }}" class="project-link">Learn More →</a>
      </article>
      {% endfor %}
    </div>
  </div>
</section>

<section id="contact" class="section section-alt">
  <div class="container">
    <h2 class="section-title">Let's Connect</h2>
    <div class="contact-content">
      <p class="contact-intro">I'm always interested in hearing about new opportunities and collaborations.</p>
      <div class="contact-links">
        <a href="mailto:{{ site.email }}" class="contact-link">
          <svg class="icon" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2">
            <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
            <polyline points="22,6 12,13 2,6"></polyline>
          </svg>
          Email
        </a>
        <a href="https://github.com/{{ site.github_username }}" target="_blank" rel="noopener noreferrer" class="contact-link">
          <svg class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
          </svg>
          GitHub
        </a>
        <a href="https://linkedin.com/in/{{ site.linkedin_username }}" target="_blank" rel="noopener noreferrer" class="contact-link">
          <svg class="icon" viewBox="0 0 24 24" fill="currentColor">
            <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
          </svg>
          LinkedIn
        </a>
      </div>
    </div>
  </div>
</section>
