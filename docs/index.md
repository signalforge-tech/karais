---
title: KARAIS — Your Real-Time AI Assistant
layout: default
---

<style>
/* Basic dark theme */
body {
    background-color: #0d0f12;
    color: #e8e8e8;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Oxygen,
                 Ubuntu, Cantarell, "Fira Sans", "Droid Sans", "Helvetica Neue",
                 sans-serif;
    line-height: 1.7;
}

/* Signal//Forge teal */
a {
    color: #19C6FF;
    font-weight: 600;
}

h1, h2, h3 {
    color: #ffffff;
    letter-spacing: 0.4px;
}

/* Center hero */
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

/* Navigation buttons */
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
    text-decoration: none;
    font-size: 1rem;
    transition: 0.15s ease-in-out;
}

.nav-btn:hover {
    background: #19C6FF;
    color: #0d0f12;
}

/* Content section */
.content {
    max-width: 800px;
    margin: 60px auto;
    padding: 0 20px;
}
</style>

<div class="hero">
    <div class="hero-title">KARAIS — Your Real-Time AI Assistant</div>
    <div class="hero-subtitle">A fully local, GPU-accelerated AI system with training, memory, and orchestration.</div>

    <div class="nav-grid">
        <a class="nav-btn" href="KARAIS_Topology_V1.md">Topology Overview</a>
        <a class="nav-btn" href="architecture/overview.md">Architecture</a>
        <a class="nav-btn" href="training/sft_plan.md">Training</a>
        <a class="nav-btn" href="memory/vector_db.md">Memory System</a>
        <a class="nav-btn" href="orchestration/scheduler_overview.md">Orchestration</a>
        <a class="nav-btn" href="roadmap/V1.md">Roadmap</a>
    </div>
</div>

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

## 🧱 System Goals

- Real-time reasoning  
- Total data ownership  
- Full offline capability  
- Modular VM-based design  
- Personal long-term memory  
- High-performance GPU workloads  
- Scalable into a cluster (V2–V3)

## 🗂 Documentation Navigation

Use the buttons above to access all technical documents.

KARAIS is under active development — new modules, diagrams, and training pipelines will be added continuously.
</div>
