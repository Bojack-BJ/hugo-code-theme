+++
authors = ["Xiaotong Li"]
title = "Building Explicit World Model for Open-world Object Manipulation"
date = "2025-10-22"
description = "Master thesis"
tags = [
    "open-world",
    "world model",
    "manipulation",
]
categories = [
    "Research Project"
]
series = ["Research Project"]
+++


<!--more-->

Open-world object manipulation has emerged as a popular research frontier in robotics. While recent advances in vision-language-action (VLA) models have achieved impressive results, they typically rely on large amounts of task-specific action data for training. This thesis aims to enable a manipulator to perform open-world object manipulation tasks without any action demonstrations. Instead of learning direct action mappings, we focus on understanding object dynamics.

<div style="text-align:center">
  <img height=auto width=auto src=../../images/thesis.png>
</div>

To this end, we propose a novel framework that builds an explicit world model for open-world object manipulation. The framework integrates open-set segmentation and grasping, 3D digital twin reconstruction, and simulation-based strategy sampling within a unified framework. At the core of our approach lies the construction of a physically grounded digital twin of the environment, which enables the framework to simulate and evaluate diverse interaction strategies before real-world execution.
Experimentally, the proposed framework is able to perform multiple open-set manipulation tasks, such as “put the banana into the basket”, “stack the green cube onto the yellow cube”, and “place the blue cup upside on the wooden box”. These results are obtained without any task-specific action demonstrations, demonstrating strong generalization and autonomy compared to existing closed-set or imitation-based systems.

<p class="project-download">
  <a class="project-download__link" href="../../uploads/Thesis.pdf" target="_blank" rel="noopener">
    Download full thesis (PDF)
  </a>
</p>

<div class="video-carousel" data-carousel>
  <p class="video-carousel__corner-title">Put an object into a container</p>
  <div class="video-carousel__viewport" data-carousel-track>
    <figure class="video-carousel__slide" data-title="Put lemon into cup">
      <video class="video-carousel__media" controls>
        <source src="../../uploads/lemon-cup.MOV" type="video/quicktime">
        Your browser does not support the video tag.
      </video>
    </figure>
    <figure class="video-carousel__slide" data-title="Put cube into box">
      <video class="video-carousel__media" controls>
        <source src="../../uploads/cube-box.MOV" type="video/quicktime">
        Your browser does not support the video tag.
      </video>
    </figure>
    <figure class="video-carousel__slide" data-title="Put cube into can">
      <video class="video-carousel__media" controls>
        <source src="../../uploads/cube-can.MOV" type="video/quicktime">
        Your browser does not support the video tag.
      </video>
    </figure>
  </div>
  <div class="video-carousel__meta">
    <span class="video-carousel__title" data-carousel-title>Blue Cup</span>
  </div>
  <div class="video-carousel__controls">
    <button class="video-carousel__arrow" type="button" aria-label="Previous video" data-carousel-prev>&larr;</button>
    <div class="video-carousel__dots" data-carousel-dots></div>
    <button class="video-carousel__arrow" type="button" aria-label="Next video" data-carousel-next>&rarr;</button>
  </div>
</div>

<div class="video-carousel" data-carousel>
  <p class="video-carousel__corner-title">Stack objects</p>
  <div class="video-carousel__viewport" data-carousel-track>
    <figure class="video-carousel__slide" data-title="Put cup on box">
      <video class="video-carousel__media" controls>
        <source src="../../uploads/cup-box.mp4" type="video/quicktime">
        Your browser does not support the video tag.
      </video>
    </figure>
    <figure class="video-carousel__slide" data-title="Put cultery on box">
      <video class="video-carousel__media" controls>
        <source src="../../uploads/cultery2.MOV" type="video/quicktime">
        Your browser does not support the video tag.
      </video>
    </figure>
    <figure class="video-carousel__slide" data-title="Stack two cubes">
      <video class="video-carousel__media" controls>
        <source src="../../uploads/stack_cube.mp4" type="video/quicktime">
        Your browser does not support the video tag.
      </video>
    </figure>
  </div>
  <div class="video-carousel__meta">
    <span class="video-carousel__title" data-carousel-title>Blue Cup</span>
  </div>
  <div class="video-carousel__controls">
    <button class="video-carousel__arrow" type="button" aria-label="Previous video" data-carousel-prev>&larr;</button>
    <div class="video-carousel__dots" data-carousel-dots></div>
    <button class="video-carousel__arrow" type="button" aria-label="Next video" data-carousel-next>&rarr;</button>
  </div>
</div>

<style>
.project-download {
  margin: 1.5rem auto 0;
  text-align: center;
}

.project-download__link {
  display: inline-flex;
  align-items: center;
  gap: 0.4rem;
  padding: 0.65rem 1.4rem;
  border-radius: 999px;
  border: 1px solid rgba(255, 255, 255, 0.35);
  color: #1e2969ff;
  font-weight: 600;
  text-decoration: none;
  transition: transform 0.2s ease, background 0.2s ease;
}

.project-download__link:hover {
  background: rgba(30, 41, 105, 0.08);
  transform: translateY(-1px);
}

.video-carousel {
  margin: 2rem auto;
  max-width: 980px;
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.video-carousel__corner-title {
  /* align-self: flex-end; */
  display: flex;
  align-items: center;
  justify-content: center;
  margin: 0;
  font-size: 2.15rem;
  font-weight: 600;
  color: #1e2969ff;
  /* text-transform: none; */
  text-align: center;
}

.video-carousel__meta {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  gap: 0.4rem;
  font-size: 0.7rem;
  color: #010101ff;
  text-align: center;
}

.video-carousel__title {
  font-size: 1.9rem;
  font-weight: 600;
  text-transform: none;
  letter-spacing: 0.01em;
}

.video-carousel__viewport {
  display: flex;
  overflow: hidden;
  border-radius: 16px;
  background: rgba(255, 255, 255, 0.03);
  scroll-behavior: smooth;
  scroll-snap-type: x mandatory;
}

.video-carousel__slide {
  flex: 0 0 100%;
  margin: 0;
  padding: 1rem;
  box-sizing: border-box;
  scroll-snap-align: center;
  text-align: center;
}

.video-carousel__media {
  width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 10px 35px rgba(0, 0, 0, 0.35);
}

.video-carousel__slide figcaption {
  margin-top: 0.75rem;
  font-size: 0.9em;
  color: #9ea3b4;
}

.video-carousel__controls {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.75rem;
  flex-wrap: wrap;
}

.video-carousel__arrow {
  border: none;
  background: #33384a;
  color: #f6f7fb;
  width: 44px;
  height: 44px;
  border-radius: 50%;
  font-size: 1.2rem;
  cursor: pointer;
  transition: transform 0.2s ease, opacity 0.2s ease;
}

.video-carousel__arrow:disabled {
  opacity: 0.35;
  cursor: not-allowed;
}

.video-carousel__arrow:not(:disabled):hover {
  transform: translateY(-2px);
}

.video-carousel__dots {
  display: flex;
  gap: 0.5rem;
}

.video-carousel__dot {
  width: 12px;
  height: 12px;
  border-radius: 50%;
  border: none;
  background: rgba(255, 255, 255, 0.25);
  cursor: pointer;
  transition: transform 0.2s ease, background 0.2s ease;
}

.video-carousel__dot.is-active {
  background: #7cb7ff;
  transform: scale(1.2);
}

@media (min-width: 960px) {
  .video-carousel__slide {
    padding: 1.5rem 2rem;
  }
}
</style>

<script>
(function () {
  const carousels = document.querySelectorAll('[data-carousel]');
  carousels.forEach((carousel) => {
    const track = carousel.querySelector('[data-carousel-track]');
    const slides = Array.from(track.children);
    const prev = carousel.querySelector('[data-carousel-prev]');
    const next = carousel.querySelector('[data-carousel-next]');
    const dotsContainer = carousel.querySelector('[data-carousel-dots]');
    const titleEl = carousel.querySelector('[data-carousel-title]');
    const slideCount = slides.length;

    slides.forEach((_, index) => {
      const dot = document.createElement('button');
      dot.type = 'button';
      dot.className = 'video-carousel__dot';
      dot.setAttribute('aria-label', `Go to video ${index + 1}`);
      dotsContainer?.appendChild(dot);
    });
    const dots = dotsContainer ? Array.from(dotsContainer.children) : [];

    const clamp = (value) => Math.min(Math.max(value, 0), slideCount - 1);
    let currentIndex = 0;

    const goTo = (index) => {
      const clampedIndex = clamp(index);
      currentIndex = clampedIndex;
      const offset = clampedIndex * track.clientWidth;
      track.scrollTo({ left: offset, behavior: 'smooth' });
      prev.disabled = clampedIndex === 0;
      next.disabled = clampedIndex === slideCount - 1;
      if (titleEl) {
        titleEl.textContent = slides[clampedIndex]?.dataset.title || '';
      }
      dots.forEach((dot, dotIndex) => {
        dot.classList.toggle('is-active', dotIndex === clampedIndex);
      });
    };

    prev.addEventListener('click', () => goTo(currentIndex - 1));
    next.addEventListener('click', () => goTo(currentIndex + 1));
    window.addEventListener('resize', () => goTo(currentIndex));

    dots.forEach((dot, index) => {
      dot.addEventListener('click', () => goTo(index));
    });

    goTo(0);
  });
})();
</script>

<!-- https://github.com/PatrickYang-5/MPC_drones

Paper PDF [here](../../uploads/mpc.pdf) -->

