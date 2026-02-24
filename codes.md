---
layout: page
title: Codes
subtitle: What I cannot create, I do not understand. - R. Feynman.
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(380px, 1fr));
  gap: 2.5rem;
  margin: 3rem 0;
  padding: 0;
}

.project-card {
  background: var(--bg-secondary);
  border: 1px solid var(--border-light);
  border-radius: 1rem;
  overflow: hidden;
  transition: all 0.3s ease;
  display: flex;
  flex-direction: column;
  height: 100%;
}

.project-card:hover {
  border-color: var(--border-color);
  box-shadow: var(--shadow-lg);
  transform: translateY(-8px);
}

.project-thumbnail {
  width: 100%;
  height: 280px;
  background-size: cover;
  background-position: center;
  position: relative;
  overflow: hidden;
}

.project-thumbnail::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  height: 50%;
  background: linear-gradient(to top, rgba(0,0,0,0.3), transparent);
}

.thumb-tsfm {
  background-image: url('https://api.dicebear.com/7.x/shapes/svg?seed=tsfm&backgroundColor=3b82f6,8b5cf6&scale=120');
  background-color: #eff6ff;
}

.thumb-ttm {
  background-image: url('https://api.dicebear.com/7.x/shapes/svg?seed=timemixer&backgroundColor=10b981,06b6d4&scale=120');
  background-color: #ecfdf5;
}

.thumb-patchtst {
  background-image: url('https://api.dicebear.com/7.x/shapes/svg?seed=transformer&backgroundColor=f59e0b,f97316&scale=120');
  background-color: #fffbeb;
}

.thumb-patchtsmixer {
  background-image: url('https://api.dicebear.com/7.x/shapes/svg?seed=mixer&backgroundColor=ec4899,a855f7&scale=120');
  background-color: #fdf4ff;
}

.thumb-foundation {
  background-image: url('https://api.dicebear.com/7.x/shapes/svg?seed=foundation&backgroundColor=6366f1,8b5cf6&scale=120');
  background-color: #eef2ff;
}

.thumb-speaker {
  background-image: url('https://api.dicebear.com/7.x/shapes/svg?seed=speaker&backgroundColor=ef4444,f97316&scale=120');
  background-color: #fef2f2;
}

.project-content {
  padding: 2.5rem;
  flex-grow: 1;
  display: flex;
  flex-direction: column;
  background: var(--bg-secondary);
}

.project-date {
  color: var(--text-tertiary);
  font-size: 0.9375rem;
  font-weight: 600;
  margin-bottom: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.project-title {
  font-size: 1.625rem;
  font-weight: 700;
  color: var(--text-primary);
  margin: 0 0 1rem;
  line-height: 1.3;
}

.project-description {
  color: var(--text-secondary);
  font-size: 1.0625rem;
  line-height: 1.7;
  margin-bottom: 2rem;
  flex-grow: 1;
}

.project-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.875rem;
  margin-top: auto;
}

.project-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.75rem 1.5rem;
  background: var(--accent-color);
  color: white;
  text-decoration: none;
  border-radius: 0.5rem;
  font-size: 1rem;
  font-weight: 600;
  border: none;
  transition: all 0.2s ease;
}

.project-link:hover {
  background: var(--accent-hover);
  color: white;
  transform: translateY(-2px);
  box-shadow: 0 4px 12px rgba(59, 130, 246, 0.4);
}

.project-link::before {
  content: '→';
  font-size: 1.25rem;
}

@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
    gap: 2rem;
  }
  
  .project-content {
    padding: 2rem;
  }
  
  .project-thumbnail {
    height: 240px;
  }
}
</style>

<div class="projects-grid">

  <div class="project-card">
    <div class="project-thumbnail thumb-tsfm"></div>
    <div class="project-content">
      <div class="project-date">2023 - Present</div>
      <h3 class="project-title">IBM/TSFM</h3>
      <p class="project-description">Our open-source work in Time Series Foundation Modeling</p>
      <div class="project-links">
        <a href="https://github.com/IBM/tsfm" class="project-link" target="_blank">Try TSFM Library</a>
      </div>
    </div>
  </div>

  <div class="project-card">
    <div class="project-thumbnail thumb-ttm"></div>
    <div class="project-content">
      <div class="project-date">April 2024</div>
      <h3 class="project-title">IBM TinyTimeMixers (TTM)</h3>
      <p class="project-description">IBM TinyTimeMixers has been opensourced with state-of-the-art performance</p>
      <div class="project-links">
        <a href="https://huggingface.co/ibm/TTM" class="project-link" target="_blank">Hugging Face</a>
        <a href="https://github.com/IBM/tsfm/tree/main/tsfm_public/models/tinytimemixer" class="project-link" target="_blank">Source Code</a>
      </div>
    </div>
  </div>

  <div class="project-card">
    <div class="project-thumbnail thumb-patchtst"></div>
    <div class="project-content">
      <div class="project-date">February 2024</div>
      <h3 class="project-title">IBM PatchTST</h3>
      <p class="project-description">Getting started tutorial for the cutting edge time series Transformer-based model PatchTST</p>
      <div class="project-links">
        <a href="https://huggingface.co/blog/patchtst" class="project-link" target="_blank">Read Tutorial</a>
      </div>
    </div>
  </div>

  <div class="project-card">
    <div class="project-thumbnail thumb-patchtsmixer"></div>
    <div class="project-content">
      <div class="project-date">January 2024</div>
      <h3 class="project-title">IBM PatchTSMixer</h3>
      <p class="project-description">Getting started tutorial for the cutting edge time series Mixer-based model PatchTSMixer</p>
      <div class="project-links">
        <a href="https://huggingface.co/blog/patchtsmixer" class="project-link" target="_blank">Read Tutorial</a>
      </div>
    </div>
  </div>

  <div class="project-card">
    <div class="project-thumbnail thumb-foundation"></div>
    <div class="project-content">
      <div class="project-date">December 2023</div>
      <h3 class="project-title">PatchTSMixer Foundation Model</h3>
      <p class="project-description">State-of-the-art Time Series Foundation Model from IBM open-sourced in Huggingface</p>
      <div class="project-links">
        <a href="https://huggingface.co/docs/transformers/main/en/model_doc/patchtsmixer" class="project-link" target="_blank">Try it out</a>
      </div>
    </div>
  </div>

  <div class="project-card">
    <div class="project-thumbnail thumb-speaker"></div>
    <div class="project-content">
      <div class="project-date">August 2020</div>
      <h3 class="project-title">Adversarial Speaker Recognition</h3>
      <p class="project-description">One of the first implementations of adversarial attacks and defense mechanisms for speaker recognition systems</p>
      <div class="project-links">
        <a href="https://github.com/usc-sail/gard-adversarial-speaker-id" class="project-link" target="_blank">View on GitHub</a>
      </div>
    </div>
  </div>

</div>
