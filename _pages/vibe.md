---
layout: page
permalink: /vibe-projects/
title: vibe projects
description: Things I vibe code for myself, mostly skills and tools for LLM coding agents. They are side projects, not research software.
nav: true
nav_order: 5
---

<style>
  .vibe-item { display: flex; align-items: flex-start; gap: 1.25rem; margin-top: 1.75rem; }
  .vibe-thumb { flex: 0 0 200px; width: 200px; height: auto; }
  .vibe-icon { height: 130px; display: flex; align-items: center; justify-content: center; font-size: 3rem; color: var(--global-theme-color); background: var(--global-code-bg-color); }
  .vibe-body { min-width: 0; }
  .vibe-body h3 { margin-top: 0; font-size: 1.4rem; }
  .vibe-body p { margin-bottom: 0.5rem; }
  @media (max-width: 576px) {
    .vibe-item { gap: 0.9rem; }
    .vibe-thumb { flex-basis: 96px; width: 96px; }
    .vibe-icon { height: 72px; font-size: 1.8rem; }
  }
</style>

## Tools & mods

<div class="vibe-item">
  <img class="vibe-thumb rounded z-depth-1" src="/assets/img/vibe/cute-claude-cat.gif" alt="The cat look of cute-claude: a ginger cat sits beside the spinner while Claude edits a file" loading="lazy">
  <div class="vibe-body">
    <h3>cute-claude</h3>
    <p><strong>A Claude Code plugin that gives the terminal a look</strong>: a ginger cat, a wizard hamster, an illuminated manuscript, a tech-priest of the Adeptus Mechanicus, or Cortana. Each look adds an animated figure above the prompt, a motto in the status line and a light flavour to Claude's wording, and some offer full role-play. Technical details stay exact either way.</p>
    <p><code>claude plugin install cute-claude --marketplace Fuminides/cute-claude</code></p>
    <a href="https://github.com/Fuminides/cute-claude"><i class="fab fa-github"></i> GitHub Repository</a>
  </div>
</div>

<div class="vibe-item">
  <img class="vibe-thumb rounded z-depth-1" src="/assets/img/vibe/visor.png" alt="The Visor window showing a bar chart, with the history of figures in the sidebar" loading="lazy">
  <div class="vibe-body">
    <h3>Visor</h3>
    <p><strong>A small desktop window where Codex and Claude Code show you plots, images and PDF slide decks</strong> while they work from the terminal, together with the skill that tells the agent when to use it. It keeps a history of every version of a figure, follows a file as the agent regenerates it, and has a panel to ask the session that made a figure about it: right-click a point and the question carries a zoomed crop of that spot. It runs locally, with no network ports or API keys.</p>
    <a href="https://github.com/Fuminides/agent-visor"><i class="fab fa-github"></i> GitHub Repository</a>
  </div>
</div>

---

## Skills for LLM agents

<div class="vibe-item">
  <img class="vibe-thumb rounded z-depth-1" src="/assets/img/vibe/literature-wiki-home.png" alt="Home page of a literature wiki built with the skill" loading="lazy">
  <div class="vibe-body">
    <h3>Literature Wiki</h3>
    <p><strong>A skill for Codex and Claude Code that turns a curated set of research papers into a source-grounded wiki</strong>: it helps collect open-access PDFs, analyses each paper, writes cross-paper synthesis pages and a short textbook, checks that every claim points to a passage in a source, and builds an offline static site with search and KaTeX math. Five slash commands cover the usual steps: <code>/create-wiki</code>, <code>/add-papers</code>, <code>/update-wiki</code>, <code>/wiki-exams</code> and <code>/serve-wiki</code>.</p>
    <a href="https://github.com/Fuminides/literature-wiki-skill"><i class="fab fa-github"></i> GitHub Repository</a>
  </div>
</div>

<div class="vibe-item">
  <div class="vibe-thumb vibe-icon rounded z-depth-1" aria-hidden="true"><i class="fas fa-sitemap"></i></div>
  <div class="vibe-body">
    <h3>Astra + Opus</h3>
    <p><strong>A Codex skill that lets Astra act as a coordinator and hand substantial work to Claude Opus</strong> through two wrapper scripts: a worker that implements changes, and a read-only consultant for debugging and independent review. Astra keeps the planning, integration and final checks. The aim is to spend fewer Astra tokens without losing quality, so the skill also says when delegating is not worth the briefing cost.</p>
    <a href="https://github.com/Fuminides/opus-delegate"><i class="fab fa-github"></i> GitHub Repository</a>
  </div>
</div>
