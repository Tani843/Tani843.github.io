---
layout: default
title: Projects
permalink: /projects/
---

# Projects

# Research Implementation

Published research projects with full codebase availability. Each implementation demonstrates methods in Bayesian inverse problems, scientific computing, and high-dimensional sampling.

## Featured Projects

<div class="project featured">
    <div class="project-header">
        <h3>PAC-Bayes Certificates for Bayesian Inverse PDEs</h3>
        <span class="project-status">Research Implementation</span>
    </div>
    <div class="project-meta">
        <span class="project-tech">Python • Bayesian Inference • PAC-Bayes • PDE-Constrained Inverse Problems</span>
        <span class="project-date">2025</span>
    </div>
    <p class="project-description">
        End-to-end research codebase for the paper introducing PAC-Bayes generalization certificates for Bayesian inverse problems governed by partial differential equations. The implementation studies a 1D heat equation conductivity inverse problem and shows how to certify predictive risk for posterior-based estimators under mesh refinement and noisy data.
    </p>
    <div class="project-features">
        <h4>Research Contributions:</h4>
        <ul>
            <li>First PAC-Bayes framework applied to Bayesian inverse problems with PDE forward models (1D heat equation).</li>
            <li>Mesh-robust certificates that separate discretization error from statistical generalization error.</li>
            <li>Certificates defined on predictive risk, aligning guarantees with scientific quantities of interest rather than parameter error.</li>
            <li>Systematic experiment grid (1,728 runs) across noise levels, sensor layouts, and priors with zero bound violations (no optimistic certificates).</li>
            <li>Analysis of how posterior contraction, effective sample size, and mesh refinement interact with PAC-Bayes bounds.</li>
        </ul>
    </div>
    <div class="project-results">
        <h4>Technical Implementation:</h4>
        <ul>
            <li>Forward and adjoint solvers for the time-dependent heat equation with automatic gradient and Hessian construction.</li>
            <li>MAP estimation and Laplace approximation around the posterior mode with low-rank Hessian structure exploited in practice.</li>
            <li>Modular PAC-Bayes pipeline for computing KL terms, empirical risk, and certified risk for multiple priors and posteriors.</li>
            <li>Fully scripted experiment runner that reproduces the paper’s figures, tables, and JSON logs from a single configuration.</li>
            <li>Reproducible environment with pinned dependencies and deterministic seeds for all experiments.</li>
        </ul>
    </div>
    <div class="project-links">
        <a href="https://github.com/Tani843/PAC_BAYES_INVERSE_PDE" class="project-link">View Code</a>
        <a href="https://github.com/Tani843/PAC_BAYES_INVERSE_PDE/blob/main/README.md" class="project-link">Documentation</a>
        <a href="https://doi.org/10.36227/techrxiv.176170993.37005709/v1" class="project-link">Research Paper</a>
    </div>
</div>

<div class="project featured">
    <div class="project-header">
        <h3>Mixed-Precision Multigrid Solvers for PDEs</h3>
     
    </div>
    <div class="project-meta">
        <span class="project-tech">Python • Multigrid Methods • Mixed Precision • Scientific Computing</span>
        <span class="project-date">2025</span>
    </div>
    <p class="project-description">
        Experimental framework for studying mixed-precision multigrid solvers on elliptic PDEs. The project explores how assigning different floating-point precisions to grid levels and smoothers affects convergence rate, stability, and total computational cost.
    </p>
    <div class="project-features">
        <h4>Key Features:</h4>
        <ul>
            <li>Configurable V-, W-, and F-cycle multigrid schemes with interchangeable smoothers and coarse-grid solvers.</li>
            <li>Flexible precision assignment (e.g., single vs double) at each level to study accuracy–efficiency trade-offs.</li>
            <li>Support for multiple benchmark PDE problems with different boundary conditions and grid sizes.</li>
            <li>Automated convergence tracking via residual norms and estimated work units.</li>
            <li>Clear separation between discretization, multigrid hierarchy, and precision policy for easy experimentation.</li>
        </ul>
    </div>
    <div class="project-results">
        <h4>Technical Implementation:</h4>
        <ul>
            <li>Structured Python implementation of grid transfer operators, smoothers, and coarse-grid corrections.</li>
            <li>Vectorized linear algebra built on standard scientific Python libraries for reproducible experiments.</li>
            <li>Config files to sweep over grid sizes, cycle types, and precision patterns without changing code.</li>
            <li>Built-in plotting utilities for residual decay curves and cost–accuracy comparison across settings.</li>
            <li>Jekyll-based documentation site summarizing algorithms, experiments, and design choices.</li>
        </ul>
    </div>
    <div class="project-links">
        <a href="https://github.com/Tani843/Mixed_Precision_Multigrid_Solvers_for_PDEs" class="project-link">View Code</a>
        <a href="https://github.com/Tani843/Mixed_Precision_Multigrid_Solvers_for_PDEs/blob/main/README.md" class="project-link">Documentation</a>
        <a href="https://tani843.github.io/Mixed_Precision_Multigrid_Solvers_for_PDEs/" class="project-link">Live Demo</a>
    </div>
</div>

<div class="project featured">
    <div class="project-header">
        <h3>Hessian-Aware Sampling in High Dimensions</h3>
        
    </div>
    <div class="project-meta">
        <span class="project-tech">Python • MCMC • Hessian-Based Preconditioning • High-Dimensional Sampling</span>
        <span class="project-date">2025</span>
    </div>
    <p class="project-description">
        Research codebase investigating how local curvature information (Hessian and Hessian–vector products) can accelerate sampling in high-dimensional posteriors. The project benchmarks Hessian-aware samplers against vanilla MCMC on synthetic targets and inverse-problem-inspired posteriors.
    </p>
    <div class="project-features">
        <h4>Research Contributions:</h4>
        <ul>
            <li>Comparison of standard random-walk and gradient-based samplers with Hessian-preconditioned variants.</li>
            <li>Study of scaling behaviour of acceptance rates, effective sample size, and mixing as dimension grows.</li>
            <li>Interfaces designed to plug in Hessian or Hessian–vector products from PDE-constrained inverse problems.</li>
            <li>Diagnostics and visualizations highlighting when curvature information provides the most benefit.</li>
            <li>Foundational experiments to inform future Hessian-aware inference for Bayesian inverse PDEs.</li>
        </ul>
    </div>
    <div class="project-results">
        <h4>Technical Implementation:</h4>
        <ul>
            <li>Modular sampler implementations with a common API for target log-density, gradient, and curvature access.</li>
            <li>Utilities for computing ESS, autocorrelation, and Gelman–Rubin-style diagnostics.</li>
            <li>Experiment scripts for running controlled comparisons across families of Gaussian and posterior-like targets.</li>
            <li>Configurable logging and plotting for chain trajectories, marginal histograms, and convergence metrics.</li>
            <li>Static website summarizing experiments and main findings using the same Jekyll theme as the main portfolio.</li>
        </ul>
    </div>
    <div class="project-links">
        <a href="https://github.com/Tani843/Hessian_Aware_Sampling_in_High_Dimensions" class="project-link">View Code</a>
        <a href="https://github.com/Tani843/Hessian_Aware_Sampling_in_High_Dimensions/blob/main/README.md" class="project-link">Documentation</a>
        <a href="https://tani843.github.io/Hessian_Aware_Sampling_in_High_Dimensions/" class="project-link">Live Demo</a>
    </div>
</div>

---

*Interested in collaborating on any of these projects? [Get in touch](tanishagupta008@gmail.com) to discuss potential partnerships or research opportunities.*

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

.project-date {
    color: #888;
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
    content: "✓";
    position: absolute;
    left: 0;
    color: #4caf50;
    font-weight: bold;
}

.project-links {
    display: flex;
    gap: 1rem;
    flex-wrap: wrap;
}

.project-link {
    display: inline-block;
    padding: 0.5rem 1.2rem;
    background: #000;
    color: white;
    text-decoration: none;
    border-radius: 4px;
    font-size: 0.9rem;
    transition: background 0.2s;
}

.project-link:hover {
    background: #333;
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
