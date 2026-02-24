---
layout: page
title: Codes
subtitle: What I cannot create, I do not understand. - R. Feynman.
---

<style>
.projects-grid {
  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(350px, 1fr));
  gap: 2rem;
  margin: 3rem 0;
}

.project-card {
  background: white;
  border: 1px solid #e8e8e8;
  border-radius: 0.75rem;
  overflow: hidden;
  transition: all 0.2s ease;
  display: flex;
  flex-direction: column;
  height: 100%;
}

.project-card:hover {
  border-color: #d4d4d4;
  box-shadow: 0 8px 24px rgba(0, 0, 0, 0.12);
  transform: translateY(-4px);
}

.project-thumbnail {
  background: linear-gradient(135deg, #2d6cdf 0%, #1e5bc6 100%);
  height: 200px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 4rem;
  color: white;
  position: relative;
  overflow: hidden;
}

.project-thumbnail::before {
  content: '';
  position: absolute;
  top: -50%;
  left: -50%;
  width: 200%;
  height: 200%;
  background: radial-gradient(circle, rgba(255,255,255,0.1) 0%, transparent 70%);
  animation: pulse 3s ease-in-out infinite;
}

@keyframes pulse {
  0%, 100% { transform: scale(1); opacity: 0.5; }
  50% { transform: scale(1.1); opacity: 0.8; }
}

.project-content {
  padding: 2rem;
  flex-grow: 1;
  display: flex;
  flex-direction: column;
}

.project-date {
  color: #737373;
  font-size: 0.9375rem;
  font-weight: 500;
  margin-bottom: 0.75rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
}

.project-title {
  font-size: 1.5rem;
  font-weight: 600;
  color: #1a1a1a;
  margin: 0 0 1rem;
  line-height: 1.3;
}

.project-description {
  color: #4a4a4a;
  font-size: 1.0625rem;
  line-height: 1.6;
  margin-bottom: 1.5rem;
  flex-grow: 1;
}

.project-links {
  display: flex;
  flex-wrap: wrap;
  gap: 0.75rem;
  margin-top: auto;
}

.project-link {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.625rem 1.25rem;
  background: #f7f7f7;
  color: #1a1a1a;
  text-decoration: none;
  border-radius: 0.5rem;
  font-size: 0.9375rem;
  font-weight: 500;
  border: 1px solid #e8e8e8;
  transition: all 0.2s ease;
}

.project-link:hover {
  background: #2d6cdf;
  color: white;
  border-color: #2d6cdf;
  transform: translateY(-2px);
}

.project-link::before {
  content: '→';
  font-size: 1.125rem;
}

@media (max-width: 768px) {
  .projects-grid {
    grid-template-columns: 1fr;
    gap: 1.5rem;
  }
  
  .project-content {
    padding: 1.5rem;
  }
}
</style>

<div class="projects-grid">

  <div class="project-card">
    <div class="project-thumbnail">🚀</div>
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
    <div class="project-thumbnail">📉</div>
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
    <div class="project-thumbnail">📘</div>
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
    <div class="project-thumbnail">📕</div>
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
    <div class="project-thumbnail">🔬</div>
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
    <div class="project-thumbnail">🗣️</div>
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
