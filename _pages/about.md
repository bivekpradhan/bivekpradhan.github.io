---
layout: about
title: About
permalink: /
subtitle: Assistant Professor of Physics | Solar Physicist | Career Mentor

profile:
  align: right
  image: prof_pic.jpg
  image_circular: true # crops the image to make it circular
  more_info: >

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: false # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: true
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

<style>
  .about-lead { font-size: 1.2rem; line-height: 1.75; max-width: 65ch; margin-bottom: 1.75rem; }
  .about-lead strong { color: var(--global-theme-color); font-weight: 600; }

  .about-columns { display: grid; grid-template-columns: 1fr 1fr; gap: 2rem; margin-bottom: 2rem; }
  .about-columns h3 { font-size: 1.15rem; margin: 0 0 0.5rem; color: var(--global-theme-color); }
  .about-columns p { margin: 0 0 1rem; line-height: 1.7; }
  .about-columns > div + div { padding-left: 2rem; border-left: 1px solid var(--global-divider-color); }

  /* Clickable heading link */
  .about-columns h3 a.heading-link {
    display: inline;
    color: var(--global-theme-color);
    text-decoration: none;
    background-image: linear-gradient(color-mix(in srgb, var(--global-theme-color) 35%, transparent), color-mix(in srgb, var(--global-theme-color) 35%, transparent));
    background-repeat: no-repeat;
    background-position: 0 92%;
    background-size: 100% 0.5em;
    padding: 0 0.15em;
    transition: background-size 0.2s ease, color 0.2s ease;
  }
  .about-columns h3 a.heading-link i { font-size: 0.7em; margin-left: 0.3em; vertical-align: 0.1em; }
  .about-columns h3 a.heading-link:hover,
  .about-columns h3 a.heading-link:focus-visible {
    background-size: 100% 100%;
    color: var(--global-hover-color);
  }
  .about-columns h3 a.heading-link:focus-visible { outline: 2px solid var(--global-theme-color); outline-offset: 3px; }

  .topic-list { display: flex; flex-wrap: wrap; gap: 0.5rem; padding: 0; margin: 0; list-style: none; }
  .topic-list li {
    padding: 0.3rem 0.85rem;
    border: 1px solid var(--global-divider-color);
    border-radius: 999px;
    font-size: 0.92rem;
    color: var(--global-text-color);
  }

  .about-invite {
    padding: 1.1rem 1.4rem;
    border: 1px dashed var(--global-divider-color);
    border-radius: 12px;
    line-height: 1.7;
  }

  @media (max-width: 768px) {
    .about-columns { grid-template-columns: 1fr; gap: 1.25rem; }
    .about-columns > div + div { padding-left: 0; border-left: 0; padding-top: 1.25rem; border-top: 1px solid var(--global-divider-color); }
    .about-lead { font-size: 1.1rem; }
  }
</style>

<p class="about-lead">
Hello, and welcome to my website. I'm <strong>Bivek Pradhan</strong>, an Assistant Professor of Physics and a researcher with a passion for education, mentorship, and career development.
</p>

<div class="about-columns">
  <div>
    <h3><a class="heading-link" href="https://bivekpradhan.github.io/assets/html/solar-corona-explainer.html" target="_blank" rel="noopener">My Research Interest<i class="fa-solid fa-arrow-up-right-from-square" aria-hidden="true"></i></a></h3>
    <p>I study the enduring puzzle of coronal heating by combining analytical theory, numerical simulations, and computational techniques.</p>
    <ul class="topic-list">
      <li>Magnetohydrodynamics</li>
      <li>Alfvén waves</li>
      <li>Compressible plasma turbulence</li>
      <li>Coronal heating</li>
      <li>Physics-informed neural networks</li>
    </ul>
  </div>
  <div>
    <h3>Teaching and mentoring</h3>
    <p>I enjoy making physics engaging and accessible, while helping students discover meaningful academic and career opportunities. My aim is to empower them to look beyond generic job titles and understand the real-world impact, possibilities, and everyday work that can make a career truly fulfilling.</p>
  </div>
</div>

<div class="about-invite">
Whether you're a student, fellow researcher, educator, or simply curious about physics, I hope you find something here that sparks your curiosity. To discuss research, exchange ideas, seek academic guidance, or collaborate, feel free to get in touch.
</div>
