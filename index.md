---
layout: default
title: Tanisha Gupta
---

<div class="landing-container">
    <!-- Header Section -->
    <header class="landing-header">
        <h1>Tanisha Gupta</h1>
        <p class="header-subtitle">PhD Applicant in Applied Mathematics</p>
        <p class="header-focus">Advancing Bayesian Inverse Problems · Scientific Computing · Uncertainty Quantification</p>
    </header>

   <!-- About Me Section -->
<section class="about-section">
    <div class="about-content">
         <p>I am a researcher in <strong>Applied Mathematics</strong> and <strong>Scientific Computing</strong>, focusing on the intersection of <strong>Bayesian inverse problems</strong>, <strong>PAC-Bayesian learning theory</strong>, and <strong>partial differential equations (PDEs)</strong>. My ongoing work develops <em>finite-sample generalization frameworks</em> for PDE-governed inverse problems, bridging rigorous mathematics with data-driven inference.</p>
        
        <p>I hold a BSc in Mathematics (University of Delhi) and an MSc in Data Science (University of Liverpool, UK). I previously worked as a Business Intelligence Analyst at <strong>Allpay Ltd (UK)</strong>, applying quantitative and computational methods to real-world data systems. I am currently a <strong>Research Assistant at Janki Devi Memorial College, University of Delhi</strong>, working on applied mathematics research and computational modeling. I aim to pursue a PhD starting Fall 2026 in Applied Mathematics or Scientific Computing, focusing on uncertainty quantification and high-performance Bayesian inference.</p>
    </div>

        <!-- Research Interests -->
      <div class="interests-section">
          <h3>Research Interests</h3>
          <div class="interests-grid">
              <span class="interest-tag">Bayesian Inverse Problems</span>
              <span class="interest-tag">Uncertainty Quantification</span>
              <span class="interest-tag">PAC-Bayesian Learning</span>
              <span class="interest-tag">Scientific Computing</span>
              <span class="interest-tag">Numerical Analysis</span>
              <span class="interest-tag">PDE-Constrained Optimization</span>
            </div>
        </div>
    </section>

    <!-- Quick Navigation -->
    <section class="nav-section">
        <div class="nav-buttons">
            <a href="/projects" class="nav-btn">Projects</a>
          <a href="/publications" class="nav-btn">Publications</a>
          <a href="/cv" class="nav-btn">CV</a>
        </div>
    </section>

    <!-- CV Section -->
    <section class="cv-section">
        <h2>Curriculum Vitae</h2>
        <p>View my professional background, experience, and skills. The CV is typeset in LaTeX for optimal readability.</p>
        
        <div class="cv-preview">
            <div class="cv-controls">
                <button onclick="zoomInCV()" class="cv-control-btn">Zoom In</button>
                <button onclick="zoomOutCV()" class="cv-control-btn">Zoom Out</button>
                <button onclick="resetZoomCV()" class="cv-control-btn">Reset Zoom</button>
                <a href="/assets/cv.pdf" download class="cv-download-btn">Download PDF</a>
            </div>
            
            <div class="pdf-viewer">
                <iframe 
                    id="cv-pdf"
                    src="/assets/cv.pdf#view=FitH"
                    width="100%" 
                    height="500"
                    frameborder="0"
                    allowfullscreen>
                </iframe>
            </div>
        </div>
    </section>

    <!-- Contact Section at Bottom -->
    <section class="contact-section">
        <h3>Get in Touch</h3>
        <div class="contact-links">
            <a href="mailto:tanishagupta008@gmail.com" class="contact-link">Email</a>
            <a href="https://github.com/Tani843" target="_blank" class="contact-link">GitHub</a>
            <a href="https://www.linkedin.com/in/tanishagupta008/" target="_blank" class="contact-link">LinkedIn</a>
        </div>
    </section>
</div>

<style>
.landing-container {
    max-width: 900px;
    margin: 0 auto;
    padding: 2rem 1rem;
    line-height: 1.6;
}

.landing-header {
    text-align: center;
    margin-bottom: 3rem;
    padding-bottom: 2rem;
    border-bottom: 2px solid #f0f0f0;
}

.landing-header h1 {
    font-size: 2.8rem;
    margin-bottom: 0.5rem;
    color: #000;
    font-weight: 700;
}

.header-subtitle {
    font-size: 1.3rem;
    color: #666;
    margin-bottom: 0.5rem;
    font-weight: 500;
}

.header-focus {
    font-size: 1.1rem;
    color: #888;
    font-style: italic;
}

.about-section {
    margin-bottom: 3rem;
}

.about-content {
    margin-bottom: 2.5rem;
}

.about-content p {
    font-size: 1.1rem;
    margin-bottom: 1.2rem;
    color: #333;
}

.interests-section {
    margin-top: 2rem;
}

.interests-section h3 {
    color: #333;
    margin-bottom: 1rem;
    font-size: 1.3rem;
}

.interests-grid {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
}

.interest-tag {
    background: #000;
    color: white;
    padding: 0.5rem 1rem;
    border-radius: 20px;
    font-size: 0.9rem;
    font-weight: 500;
}

/* Navigation Section */
.nav-section {
    margin-bottom: 3rem;
}

.nav-buttons {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
}

.nav-btn {
    padding: 0.8rem 2rem;
    background: #000;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    font-size: 1rem;
    transition: background 0.2s, transform 0.2s;
    flex: 1;
    max-width: 200px;
    text-align: center;
}

.nav-btn:hover {
    background: #333;
    transform: translateY(-2px);
}

/* CV Section */
.cv-section {
    margin-bottom: 3rem;
}

.cv-section h2 {
    color: #333;
    margin-bottom: 1rem;
}

.cv-controls {
    margin-bottom: 1rem;
    text-align: center;
}

.cv-control-btn {
    padding: 0.6rem 1.2rem;
    margin: 0 0.3rem;
    background: #000;
    color: white;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    font-size: 0.9rem;
    transition: background 0.2s;
}

.cv-control-btn:hover {
    background: #333;
}

.cv-download-btn {
    padding: 0.6rem 1.2rem;
    background: #000;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    font-size: 0.9rem;
    transition: background 0.2s;
}

.cv-download-btn:hover {
    background: #333;
}

.pdf-viewer {
    border: 1px solid #eaeaea;
    border-radius: 8px;
    overflow: hidden;
    background-color: #f8f9fa;
}

/* Contact Section */
.contact-section {
    text-align: center;
    padding: 2rem 0;
    border-top: 1px solid #f0f0f0;
}

.contact-section h3 {
    color: #333;
    margin-bottom: 1.5rem;
    font-size: 1.3rem;
}

.contact-links {
    display: flex;
    gap: 1rem;
    justify-content: center;
    flex-wrap: wrap;
}

.contact-link {
    padding: 0.8rem 1.5rem;
    background: #000;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    font-size: 0.9rem;
    transition: background 0.2s;
}

.contact-link:hover {
    background: #333;
}

@media (max-width: 768px) {
    .landing-header h1 {
        font-size: 2.2rem;
    }
    
    .nav-buttons {
        flex-direction: column;
        align-items: center;
    }
    
    .nav-btn {
        width: 100%;
        max-width: 250px;
    }
    
    .cv-controls {
        display: flex;
        flex-wrap: wrap;
        gap: 0.5rem;
        justify-content: center;
    }
    
    .cv-control-btn, .cv-download-btn {
        margin: 0.2rem;
    }
    
    .contact-links {
        flex-direction: column;
        align-items: center;
    }
    
    .contact-link {
        width: 200px;
    }
}
</style>

<script>
let currentZoomCV = 1;
const zoomStepCV = 0.1;
const minZoomCV = 0.5;
const maxZoomCV = 3;

function zoomInCV() {
    if (currentZoomCV < maxZoomCV) {
        currentZoomCV += zoomStepCV;
        updateZoomCV();
    }
}

function zoomOutCV() {
    if (currentZoomCV > minZoomCV) {
        currentZoomCV -= zoomStepCV;
        updateZoomCV();
    }
}

function resetZoomCV() {
    currentZoomCV = 1;
    updateZoomCV();
}

function updateZoomCV() {
    const iframe = document.getElementById('cv-pdf');
    iframe.style.transform = `scale(${currentZoomCV})`;
    iframe.style.transformOrigin = 'top left';
    iframe.style.width = `${100 / currentZoomCV}%`;
    iframe.style.height = `${500 / currentZoomCV}px`;
}
</script>
