---
layout: default
title: Projects
permalink: /projects.html
---

<div style="margin-bottom: 30px;">
  <a href="{{ '/' | relative_url }}">🏠 Home</a> |
  <a href="{{ '/projects.html' | relative_url }}">🛠 Projects</a> |
  <a href="{{ '/contact.html' | relative_url }}">📬 Contact</a>
</div>

# 🛠 Projects (smoke test)

> Click to expand each project for details.

<style>
/* Card-like details */
details.proj {
  border: 1px solid #e5e7eb; border-radius: 12px; padding: .75rem 1rem; margin: .8rem 0;
  box-shadow: 0 2px 6px rgba(0,0,0,.04); background: #fff;
}
details.proj[open] { background: #fafafa; }
details.proj > summary {
  cursor: pointer; list-style: none; font-weight: 600; display: flex; align-items: center;
}
details.proj > summary::-webkit-details-marker { display: none; }
details.proj > summary .meta {
  font-weight: 400; color: #6b7280; margin-left: .5rem; font-size: .95rem;
}
details.proj > summary::after {
  content: "▸"; margin-left: auto; transition: transform .2s ease;
}
details.proj[open] > summary::after { transform: rotate(90deg); }
/* Small badge styles */
.badge { display:inline-block; padding:.12rem .45rem; border:1px solid #e5e7eb; border-radius:999px; font-size:.8rem; color:#374151; margin-right:.35rem;}
/* Section headers */
.h2line { margin-top: 1.6rem; border-top: 1px solid #eee; padding-top: .8rem; }
.controls { margin: .6rem 0 1rem; }
.controls button {
  border: 1px solid #e5e7eb; background: #fff; border-radius: 8px; padding: .35rem .65rem; cursor: pointer;
}
.controls button:hover { background:#f9fafb; }
</style>

<div class="controls">
  <button id="expandAll">Expand all</button>
  <button id="collapseAll">Collapse all</button>
</div>

<script>
document.addEventListener('DOMContentLoaded', function() {
  const all = Array.from(document.querySelectorAll('details.proj'));
  const openAll = () => all.forEach(d => d.open = true);
  const closeAll = () => all.forEach(d => d.open = false);
  const ex = document.getElementById('expandAll');
  const co = document.getElementById('collapseAll');
  if (ex) ex.addEventListener('click', openAll);
  if (co) co.addEventListener('click', closeAll);
});

## Industry Collaboration Project {#industry}

<details class="proj">
  <summary>Flexible Lubricator Handling & Inspection Platform
    <span class="meta">– 5-DOF gantry, flexible gripper, inspection workflow</span>
  </summary>
  <p><strong>Role:</strong> Lead Mechanical Engineer</p>
  <p>
    <span class="badge">SolidWorks</span>
    <span class="badge">ANSYS</span>
    <span class="badge">MATLAB/Simulink</span>
    <span class="badge">Coupled/Fuzzy PID</span>
  </p>
  <ul>
    <li>Modular 5-DOF gantry with vision-assisted flexible gripper for ≈200-lb lubricators.</li>
    <li>Structural optimization & flipping platform; verified on a 2:1 prototype.</li>
    <li>Real-time object detection → automated inspection flow.</li>
  </ul>
  <p><a href="/projects/lubricator/">Read more »</a></p>
</details>
</script>

