---
title: KARAIS — Your Real-Time AI Assistant
layout: default
---

<style>

/* ----------------------------- */
/* Global dark theme styling     */
/* ----------------------------- */

body {
    background-color: #0d0f12;
    color: #e8e8e8;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
                 Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue",
                 sans-serif;
    line-height: 1.7;
    margin: 0;
    padding: 0;
}

a {
    color: #19C6FF;
    font-weight: 600;
    text-decoration: none;
}

h1, h2, h3 {
    color: #ffffff;
    letter-spacing: 0.4px;
}

/* ----------------------------- */
/* Brand Row Fix                 */
/* ----------------------------- */

.brand-row {
    display: flex !important;
    align-items: center !important;
    gap: 14px !important;
    margin-bottom: 0 !important;
    padding-bottom: 0 !important;
}

/* ----------------------------- */
/* Animated Slash                */
/* ----------------------------- */

.io-slash {
    color: #19C6FF;
    display: inline-block;
    animation: slashPulse 1.8s ease-in-out infinite;
    will-change: opacity, transform;
}

@keyframes slashPulse {
    0%   { opacity: 0.6; transform: translateY(0px); }
    50%  { opacity: 1.0; transform: translateY(-1px) scale(1.02); }
    100% { opacity: 0.6; transform: translateY(0px); }
}

/* ----------------------------- */
/* Hero section                  */
/* ----------------------------- */

.hero {
    text-align: center;
    padding: 60px 20px 40px 20px;
    border-bottom: 1px solid #222831;
}

.hero-title {
    font-size: 2.8rem;
    font-weight: 700;
    margin-bottom: 12px;
}

.hero-subtitle {
    font-size: 1.2rem;
    color: #b5b5b5;
    font-weight: 300;
    margin-bottom: 40px;
}

/* ----------------------------- */
/* Navigation buttons            */
/* ----------------------------- */

.nav-grid {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 16px;
    margin-top: 30px;
}

.nav-btn {
    background: #111318;
    border: 1px solid #19C6FF;
    padding: 14px 24px;
    border-radius: 10px;
    font-size: 1rem;
    transition: 0.2s ease-in-out;
}

.nav-btn:hover {
    background: #19C6FF;
    color: #0d0f12;
}

/* ----------------------------- */
/* Content container             */
/* ----------------------------- */

.content {
    max-width: 800px;
    margin: 60px auto;
    padding: 0 20px;
}

</style>


<!-- ============================ -->
<!-- Signal//Forge Branding Header -->
<!-- ============================ -->

<div style="
    width: 100%;
    padding: 40px 20px 10px 20px;
    text-align: left;
    border-bottom: 1px solid #222831;
    max-width: 1200px;
    margin: 0 auto;
">

    <div class="brand-row">

        <!-- Signal//Forge Wordmark -->
        <div style="font-size: 1.8rem; font-weight: 700; color: #ffffff; letter-spacing: 0.5px; font-family: inherit;">
            SIGNAL<span style="color:#19C6FF;">//</span>FORGE
        </div>

        <!-- Animated I/O signature -->
        <div style="font-size: 1.4rem; font-weight: 600; display: flex; gap: 4px;">
            <span style="color: #ffffff;">I</span>
            <span class="io-slash" style="color:#19C6FF;">/</span>
            <span style="color: #ffffff;">O</span>
        </div>

    </div>

</div>


<!-- ----------------------------- -->
<!-- Hero Section -->
<!-- ----------------------------- -->

<div class="hero">
    <div class="hero-title">KARAIS — Your Real-Time AI Assistant</div>
    <div class="hero-subtitle">
        A fully local, GPU-accelerated AI system with training, memory, and orchestration.
    </div>

    <div class="nav-grid">
        <a class="nav-btn" href="KARAIS_Topology_V1.md">Topology Overview</a>
        <a class="nav-btn" href="architecture/overview.md">Architecture</a>
        <a class="nav-btn" href="training/sft_plan.md">Training</a>
        <a class="nav-btn" href="memory/vector_db.md">Memory System</a>
        <a class="nav-btn" href="orchestration/scheduler_overview.md">Orchestration</a>
        <a class="nav-btn" href="roadmap/V1.md">Roadmap</a>
    </div>
</div>


<!-- ----------------------------- -->
<!-- Main content section (optional) -->
<!-- ----------------------------- -->

<div class="content">

## ⚡ What is KARAIS?

KARAIS is a fully local AI assistant built on:

- GPU-accelerated training & inference  
- Proxmox-based VM cluster (Brain, Trainer, Worker)  
- ZFS-backed storage  
- Vector memory + RAG indexing  
- Custom LoRA/SFT training  
- Expandable multi-node design  

This documentation outlines the architecture, memory system, training pipelines, and long-term engineering roadmap.

</div>

<!-- ----------------------------- -->
<!-- Footer                        -->
<!-- ----------------------------- -->

<div style="
    text-align: center;
    padding: 40px 20px 60px 20px;
    color: #b5b5b5;
    margin-top: 60px;
    border-top: 1px solid #222831;
">

    <div style="font-size: 1rem; margin-bottom: 6px; font-weight: 600;">

        <!-- Signal//Forge Wordmark (Footer Version) -->
        <span style="color: #ffffff;">SIGNAL</span>
        <span style="color:#19C6FF;">//</span>
        <span style="color: #ffffff;">FORGE</span>
    </div>

    <div style="font-size: 0.9rem; color: #777777; margin-top: 4px;">
        © 2025 Signal//Forge  
    </div>

    <div style="font-size: 0.85rem; color: #555555; margin-top: 6px;">
        Built with love, GPUs, and too many late nights.
    </div>

</div>

