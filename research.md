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
        <span class="project-tech">Applied Mathematics • Scientific Computing • PAC-Bayesian Learning</span>
    </div>
    
    <p class="project-description">
        My research is centered on <strong>Bayesian inverse problems</strong> and <strong>uncertainty quantification</strong> for systems governed by <strong>partial differential equations (PDEs)</strong>. I am particularly interested in developing <em>PAC-Bayesian generalization frameworks</em> for PDE-based inverse problems, providing finite-sample guarantees on predictive error and bridging modern learning theory with classical numerical analysis.
    </p>

    <div class="project-features">
        <h4>The Challenge with Bayesian Inversion</h4>
        <ul>
            <li><strong>Ill-posedness:</strong> small perturbations in noisy data can lead to large changes in inferred parameters.</li>
            <li><strong>High-dimensional posteriors:</strong> PDE-based models often require estimating spatially varying fields or many parameters, making sampling and inference computationally expensive.</li>
            <li><strong>Lack of finite-sample guarantees:</strong> classical Bayesian methods yield credible intervals, but rarely provide <em>distribution-free</em> guarantees on predictive error for new observations.</li>
            <li><strong>Mesh and discretization effects:</strong> numerical choices (grid size, time step) can significantly affect posterior behavior and stability.</li>
        </ul>
    </div>

    <div class="project-results">
        <h4>Why This Matters</h4>
        <p>These challenges appear in many real-world systems:</p>
        <ul>
            <li><strong>Heat and diffusion processes:</strong> inferring thermal conductivity or diffusion coefficients from sparse temperature measurements.</li>
            <li><strong>Subsurface and environmental modelling:</strong> determining material properties of soil or rock from indirect data.</li>
            <li><strong>Engineering and medical applications:</strong> reconstructing internal structures from boundary or sensor observations.</li>
        </ul>
        <p>In such settings, we need methods that are not only accurate, but also come with <strong>provable guarantees</strong> on how well the inferred model will generalize to new data.</p>
    </div>
</div>

<div class="project featured">
    <div class="project-header">
        <h3>Research Directions</h3>
        <span class="project-status">Current Focus</span>
    </div>

    <div class="project-features">
        <h4>1. PAC-Bayesian Certificates for Inverse PDE Problems</h4>
        <p>I am developing a PAC-Bayesian framework for <strong>PDE-governed inverse problems</strong>, starting with the one-dimensional heat equation as a case study. The goal is to derive risk bounds that connect posterior distributions to out-of-sample prediction error in a mesh-robust way.</p>
        <p><strong>Key Question:</strong> How can we obtain <em>finite-sample, distribution-free</em> guarantees for Bayesian inverse solutions in infinite-dimensional or high-dimensional PDE settings?</p>
    </div>

    <div class="project-features">
        <h4>2. Numerical Methods for High-Dimensional Posteriors</h4>
        <p>I am interested in numerical strategies that make Bayesian inversion more tractable, including Laplace approximations, Hessian-aware sampling, and careful discretization strategies that control the effect of mesh refinement on posterior behavior.</p>
        <p><strong>Key Question:</strong> What combinations of numerical solvers and approximate inference schemes yield stable, reliable posteriors with controllable error in practical computation time?</p>
    </div>

    <div class="project-features">
        <h4>3. Scientific Machine Learning & PDE-Constrained Learning</h4>
        <p>Longer-term, I aim to explore hybrid approaches that combine physics-based PDE models with data-driven components, while retaining rigorous uncertainty quantification and theoretical guarantees.</p>
        <p><strong>Key Question:</strong> How can we design learning algorithms that respect physical structure, provide calibrated uncertainty, and come with PAC-style generalization guarantees?</p>
    </div>
</div>

<div class="project featured">
    <div class="project-header">
        <h3>The Big Picture</h3>
        <span class="project-status">Research Vision</span>
    </div>
    
    <p class="project-description">
        As computational models become more complex and central to decision-making, the ability to <strong>trust</strong> their predictions becomes critical. My research vision is to build a bridge between <strong>learning theory</strong>, <strong>Bayesian statistics</strong>, and <strong>scientific computing</strong>, so that PDE-based models come with interpretable uncertainty and provable performance guarantees.
    </p>

    <div class="project-features">
        <h4>Research Objectives</h4>
        <ul>
            <li><strong>Rigorous Uncertainty Quantification</strong> – developing methods that provide mathematically sound bounds on predictive risk for Bayesian inverse problems.</li>
            <li><strong>Scalable Algorithms</strong> – designing numerical and probabilistic techniques that remain practical for high-dimensional and mesh-refined PDE systems.</li>
            <li><strong>Physics-Aware Learning</strong> – integrating physical constraints and PDE structure into learning algorithms without sacrificing theoretical guarantees.</li>
        </ul>
    </div>
<div class="project-results">
    <h4>Long-term Impact</h4>
    <p>
        My long-term research goal is to develop mathematically rigorous and computationally scalable frameworks for Bayesian inference and uncertainty quantification in complex scientific systems. I aim to contribute to a new class of reliable scientific models that remain stable under discretization, provide provable generalization guarantees, and integrate seamlessly with large-scale PDE-based simulations.
        <br><br>
        At a broader level, my work is motivated by the need for trustworthy computational tools in science and engineering—methods that combine statistical robustness with numerical precision. I aspire to advance the theoretical foundations and practical algorithms that enable transparent, reproducible, and high-confidence decision-making in high-dimensional, noisy, and uncertain environments.
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
