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


<!-- ----------------------------- -->
<!-- Hero Section -->
<!-- ----------------------------- -->
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

    <!-- Brand Row -->
    <div style="display: flex; align-items: center; gap: 14px;">

        <!-- Signal//Forge Wordmark -->
        <div style="font-size: 1.8rem; font-weight: 700; color: #ffffff; letter-spacing: 0.5px; font-family: inherit;">
            SIGNAL<span style="color:#19C6FF;">//</span>FORGE
        </div>

<!-- Animated I/O signature -->
<div style="font-size: 1.4rem; font-weight: 600; display: flex; gap: 4px;">
    <span style="color: #ffffff;">I</span>
    <span class="io-slash">/</span>
    <span style="color: #ffffff;">O</span>
</div>

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
