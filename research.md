---
layout: default
title: Research Vision
permalink: /research/
---

<div style="max-width: 800px; margin: 0 auto;">

<div class="project featured">
    <div class="project-header">
        <h3>Research Focus: Bayesian Inverse Problems & Uncertainty Quantification</h3>
        <span class="project-status">Active Research</span>
    </div>
    
    <div class="project-meta">
        <span class="project-tech">Numerical Analysis • Scientific Computing • PAC-Bayesian Inference</span>
    </div>
    
    <p class="project-description">
        My research lies at the intersection of <strong>Bayesian inverse problems</strong>, <strong>numerical analysis</strong>, and <strong>scientific computing</strong>. I study how uncertainty propagates through <strong>partial differential equation (PDE)</strong> models and develop frameworks that deliver <strong>finite-sample guarantees</strong> for inverse solutions. A central theme of my work is the use of <em>PAC-Bayesian learning theory</em> to quantify how discretization, mesh refinement, and solver approximations affect generalization behaviour in PDE-based inference.
    </p>

    <div class="project-features">
        <h4>The Challenge with Bayesian Inversion</h4>
        <ul>
            <li><strong>Ill-posedness:</strong> small perturbations in noisy data can produce large deviations in inferred model parameters, especially in PDE-governed systems.</li>
            <li><strong>High-dimensional posteriors:</strong> PDE-based models often involve spatially distributed unknowns, creating computational challenges for inference and sampling.</li>
            <li><strong>No finite-sample guarantees:</strong> classical Bayesian analysis provides credible regions but rarely offers <em>distribution-free, sample-dependent</em> bounds on predictive error.</li>
            <li><strong>Discretization sensitivity:</strong> choices such as grid resolution, time-stepping, and solver accuracy can significantly distort posterior shape and stability.</li>
        </ul>
    </div>

    <div class="project-results">
        <h4>Why This Matters</h4>
        <p>The need for <strong>trustworthy, reproducible</strong> inference arises across many scientific and engineering domains:</p>
        <ul>
            <li><strong>Heat and diffusion processes:</strong> reconstructing conductivity or diffusivity from sparse or noisy measurements.</li>
            <li><strong>Subsurface and environmental modelling:</strong> estimating underground properties from boundary data.</li>
            <li><strong>Engineering and biomedical applications:</strong> recovering internal structures using sensor or boundary observations.</li>
        </ul>
        <p>PDE-based models power these systems, but accurate solutions alone are not enough. We need methods with <strong>provable guarantees</strong>—methods that quantify how well the inferred solution will generalize to new data and how numerical choices influence uncertainty.</p>
    </div>
</div>

<div class="project featured">
    <div class="project-header">
        <h3>Research Directions</h3>
        <span class="project-status">Current Focus</span>
    </div>

    <div class="project-features">
        <h4>1. PAC-Bayesian Certificates for Inverse PDE Problems</h4>
        <p>I am developing a <strong>PAC-Bayesian generalization framework</strong> for inverse problems constrained by PDEs. Starting with the one-dimensional heat equation, I derive <strong>mesh-robust risk bounds</strong> that connect posterior uncertainty to out-of-sample predictive error. This provides a new perspective for uncertainty quantification that unifies <em>learning theory</em> with <em>classical PDE analysis</em>.</p>
        <p><strong>Key Question:</strong> Can we develop <em>finite-sample, distribution-free</em> guarantees for posterior stability in high-dimensional or infinite-dimensional PDE settings?</p>
    </div>

    <div class="project-features">
        <h4>2. Numerical Methods for High-Dimensional Posteriors</h4>
        <p>I design numerical strategies that make Bayesian inversion computationally feasible. This includes <strong>Laplace approximations</strong>, <strong>Hessian-aware sampling</strong>, and <strong>discretization-aware inference schemes</strong> that quantify how numerical error affects posterior accuracy.</p>
        <p><strong>Key Question:</strong> What combinations of solvers, discretization choices, and approximate inference methods yield posteriors that are both stable and computationally efficient?</p>
    </div>

    <div class="project-features">
        <h4>3. Scientific Machine Learning & Physics-Constrained Learning</h4>
        <p>I am exploring hybrid approaches that merge data-driven learning with PDE-constrained structure while preserving interpretability and uncertainty guarantees. My aim is to incorporate <strong>physical laws</strong> and <strong>numerical consistency</strong> into learning models without sacrificing rigorous error control.</p>
        <p><strong>Key Question:</strong> How can we design learning algorithms that respect PDE structure, provide calibrated uncertainty, and satisfy PAC-style generalization bounds?</p>
    </div>
</div>

<div class="project featured">
    <div class="project-header">
        <h3>The Big Picture</h3>
        <span class="project-status">Research Vision</span>
    </div>
    
    <p class="project-description">
        My long-term vision is to build a unified theory that connects <strong>learning-theoretic guarantees</strong> with <strong>numerical stability</strong> in PDE-based inference. Scientific simulations guide decisions in engineering, climate modelling, physics, and medicine — yet their uncertainty is often difficult to interpret or trust. I aim to create computational frameworks where <strong>accuracy, uncertainty, and generalization are mathematically linked</strong>.
    </p>

    <div class="project-features">
        <h4>Research Objectives</h4>
        <ul>
            <li><strong>Rigorous Uncertainty Quantification</strong> – deriving mathematically sound generalization bounds for inverse problems governed by PDEs.</li>
            <li><strong>Scalable Numerical Algorithms</strong> – developing methods that remain efficient for high-dimensional, mesh-refined, or computationally intensive PDE systems.</li>
            <li><strong>Physics-Structured Learning</strong> – integrating PDE constraints and numerical structure into data-driven algorithms while maintaining theoretical guarantees.</li>
        </ul>
    </div>

<div class="project-results">
    <h4>Long-term Impact</h4>
    <p>
        My long-term goal is to shape a new class of computational methods for Bayesian inference: methods that remain stable under discretization, that scale to high-dimensional settings, and that come with <strong>provable generalization guarantees</strong>. I aspire to advance the mathematical foundations needed for transparent, reproducible, and high-confidence decision-making in noisy, high-dimensional, and scientifically complex environments.
        <br><br>
        Ultimately, my vision is to establish a rigorous bridge between <strong>numerical analysis</strong>, <strong>PDE-based modelling</strong>, and <strong>learning theory</strong>, enabling trustworthy scientific computing for the next generation of data-informed simulations.
    </p>
</div>
</div>

</div>

<style>
.project {
    border: 1px solid #eaeaea;
    border-radius: 8px;
    padding: 2rem;
    margin-bottom: 2.5rem;
    transition: transform 0.2s, box-shadow 0.2s;
}

.project.featured {
    border-left: 4px solid #000;
    background: #fafafa;
}

.project:hover {
    transform: translateY(-2px);
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
}

.project-header {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    margin-bottom: 1rem;
    flex-wrap: wrap;
    gap: 1rem;
}

.project-header h3 {
    color: #000;
    margin: 0;
    font-size: 1.4rem;
    flex: 1;
    min-width: 300px;
}

.project-status {
    background: #000;
    color: white;
    padding: 0.3rem 0.8rem;
    border-radius: 4px;
    font-size: 0.9rem;
    font-weight: 500;
    white-space: nowrap;
}

.project-meta {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 1.5rem;
    flex-wrap: wrap;
    gap: 1rem;
}

.project-tech {
    color: #666;
    font-family: 'Monaco', 'Menlo', monospace;
    font-size: 0.9rem;
}

.project-description {
    color: #333;
    line-height: 1.6;
    margin-bottom: 1.5rem;
    font-size: 1.1rem;
}

.project-features, .project-results {
    margin-bottom: 1.5rem;
}

.project-features h4, .project-results h4 {
    color: #000;
    margin-bottom: 0.5rem;
    font-size: 1.1rem;
}

.project-features ul, .project-results ul {
    list-style: none;
    padding-left: 0;
}

.project-features li, .project-results li {
    padding: 0.3rem 0;
    position: relative;
    padding-left: 1.5rem;
    color: #333;
}

.project-features li:before, .project-results li:before {
    content: "•";
    position: absolute;
    left: 0;
    color: #000;
    font-weight: bold;
    font-size: 1.2rem;
}

@media (max-width: 768px) {
    .project-header {
        flex-direction: column;
        align-items: flex-start;
    }
    
    .project-header h3 {
        min-width: auto;
    }
    
    .project-meta {
        flex-direction: column;
        align-items: flex-start;
    }
}
</style>
