---
layout: default
title: Publications
permalink: /publications/
---

# Publications

Peer-reviewed research papers and preprints in Bayesian Inverse Problems, Uncertainty Quantification, and Scientific Computing.

## Featured Publication

<div class="publication featured">
    <div class="pub-header">
        <h3>PAC-Bayes Certificates for Bayesian Inverse Problems: A Case Study on the Heat Equation</h3>
        <span class="pub-status">Preprint • 2025 (Under Review at SIAM JUQ)</span>
    </div>

    <p class="pub-authors">Tanisha Gupta</p>

    <p class="pub-abstract">
        Modern Bayesian inverse methods for PDEs provide posterior distributions and credible intervals but no 
        <strong>finite-sample guarantees</strong> for prediction on new sensor data. This paper introduces the 
        first <strong>PAC-Bayes generalization framework for Bayesian inverse PDEs</strong>, using thermal 
        conductivity inference in the 1-D heat equation as a case study. By exploiting the Gibbs–posterior view 
        and a <strong>sigmoid-bounded squared loss</strong>, we derive <strong>mesh-robust PAC-Bayes certificates</strong> 
        that separate statistical generalization error from numerical discretization bias.
        <br><br>
        Across <strong>1,728 experimental configurations</strong> spanning sensor counts, noise levels, 
        temperature regimes, and mesh resolutions, all certificates satisfy 
        <code>Bλ ≥ L̂</code>. The gap between empirical and certified risk remains typically 
        <strong>3–12% (often 7–9%)</strong>, while the discretization penalty drops by <strong>≈4×</strong>
        when refining the mesh from 50 to 100 points, confirming second-order accuracy. These results demonstrate 
        that PAC-Bayes provides <strong>conservative yet practical reliability guarantees</strong> for inverse PDE 
        models—flagging overconfident posteriors under sparse sensing or high noise—and serving as a 
        <strong>modular safety layer</strong> for existing Bayesian solvers.
    </p>
    <div class="pub-links">
        <a href="https://doi.org/10.36227/techrxiv.176170993.37005709/v1" class="pub-link">Paper</a>
        <<a href="https://github.com/Tani843/PAC_BAYES_INVERSE_PDE" class="pub-link">Code</a>
        <a href="https://scholar.google.com/citations?user=QYQqZZgAAAAJ&hl=en" class="pub-link">Google Scholar</a>
    </div>
    <div class="pub-tags">
        <span class="pub-tag">Bayesian Inverse Problems</span>
        <span class="pub-tag">Uncertainty Quantification</span>
        <span class="pub-tag">PAC-Bayes Theory</span>
        <span class="pub-tag">Scientific Computing</span>
        <span class="pub-tag">PDEs</span>
    </div>
</div>



*For collaboration inquiries or early access to preprints, please <a href="mailto:tanishagupta008@gmail.com">contact me</a>.*

<style>
.publication {
    border: 1px solid #eaeaea;
    border-radius: 8px;
    padding: 2rem;
    margin-bottom: 2rem;
    transition: transform 0.2s, box-shadow 0.2s;
}

.publication.featured {
    border-left: 4px solid #000;
    background: #fafafa;
}

.publication:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.pub-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 0.5rem;
    flex-wrap: wrap;
    gap: 1rem;
}

.pub-header h3 {
    color: #000;
    margin: 0;
    font-size: 1.3rem;
    line-height: 1.4;
    flex: 1;
    min-width: 300px;
}

.pub-status {
    background: #000;
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 4px;
    font-size: 0.9rem;
    font-weight: 500;
    white-space: nowrap;
}

.pub-authors {
    color: #666;
    font-style: italic;
    margin-bottom: 1rem;
    font-size: 1rem;
}

.pub-abstract {
    color: #333;
    line-height: 1.6;
    margin-bottom: 1.5rem;
}

.pub-links {
    display: flex;
    gap: 1rem;
    margin-bottom: 1rem;
    flex-wrap: wrap;
}

.pub-link {
    display: inline-block;
    padding: 0.4rem 1rem;
    background: #000;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    font-size: 0.9rem;
    transition: background 0.2s;
}

.pub-link:hover {
    background: #333;
}

.pub-tags {
    display: flex;
    gap: 0.5rem;
    flex-wrap: wrap;
}

.pub-tag {
    background: #f0f0f0;
    color: #666;
    padding: 0.2rem 0.6rem;
    border-radius: 12px;
    font-size: 0.8rem;
}

.manuscripts-section {
    background: #fff8e1;
    padding: 2rem;
    border-radius: 8px;
    margin: 2rem 0;
    border-left: 4px solid #ffd54f;
}

.manuscript-item {
    margin-bottom: 1rem;
    padding-bottom: 1rem;
    border-bottom: 1px solid #ffe082;
}

.manuscript-item:last-child {
    border-bottom: none;
    margin-bottom: 0;
}

.manuscript-item strong {
    color: #000;
}

.manuscript-target {
    color: #666;
    font-style: italic;
    font-size: 0.9rem;
}

@media (max-width: 768px) {
    .pub-header {
        flex-direction: column;
        align-items: flex-start;
    }
    
    .pub-header h3 {
        min-width: auto;
    }
    
    .pub-status {
        align-self: flex-start;
    }
}
</style>
