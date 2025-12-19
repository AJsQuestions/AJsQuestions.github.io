---
title: "Questions"
aliases: /questions
description: "Thought experiments I think with"
---

> *I don’t keep questions because I expect answers.  
> I keep them because they change how I notice things.*

---

<!-- Constellation Map (static SVG, PaperMod-friendly) -->
<div style="max-width: 980px; margin: 1.25rem auto 1.25rem auto;">
<svg viewBox="0 0 980 520" width="100%" height="auto" role="img" aria-label="A constellation map of question clusters">
  <defs>
    <filter id="softGlow" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="2.2" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <style>
      .bg { fill: transparent; }
      .skyline { stroke: rgba(255,255,255,0.08); stroke-width: 1.25; }
      .link { stroke: rgba(255,255,255,0.14); stroke-width: 1.2; }
      .link2 { stroke: rgba(255,255,255,0.10); stroke-width: 1.0; stroke-dasharray: 3 6; }
      .node { fill: rgba(255,255,255,0.88); }
      .nodeDim { fill: rgba(255,255,255,0.65); }
      .nodeCore { fill: rgba(255,255,255,0.95); }
      .label { fill: rgba(255,255,255,0.84); font: 600 15px ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial; letter-spacing: 0.2px; }
      .sublabel { fill: rgba(255,255,255,0.55); font: 500 12.5px ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial; }
      .tiny { fill: rgba(255,255,255,0.35); font: 500 11px ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial; }
      .click { cursor: pointer; }
      .ring { fill: none; stroke: rgba(255,255,255,0.10); stroke-width: 1.0; }
    </style>
  </defs>

  <rect class="bg" x="0" y="0" width="980" height="520"/>

  <!-- faint horizon line -->
  <line class="skyline" x1="60" y1="455" x2="920" y2="455"/>

  <!-- orbital rings around core -->
  <circle class="ring" cx="490" cy="260" r="86"/>
  <circle class="ring" cx="490" cy="260" r="150"/>
  <circle class="ring" cx="490" cy="260" r="215"/>

  <!-- links to clusters -->
  <line class="link" x1="490" y1="260" x2="240" y2="145"/>
  <line class="link" x1="490" y1="260" x2="745" y2="150"/>
  <line class="link" x1="490" y1="260" x2="185" y2="320"/>
  <line class="link" x1="490" y1="260" x2="790" y2="320"/>
  <line class="link" x1="490" y1="260" x2="490" y2="85"/>
  <line class="link" x1="490" y1="260" x2="490" y2="445"/>

  <!-- secondary links (dashed) -->
  <line class="link2" x1="240" y1="145" x2="185" y2="320"/>
  <line class="link2" x1="745" y1="150" x2="790" y2="320"/>
  <line class="link2" x1="490" y1="85"  x2="745" y2="150"/>
  <line class="link2" x1="490" y1="85"  x2="240" y2="145"/>
  <line class="link2" x1="490" y1="445" x2="185" y2="320"/>
  <line class="link2" x1="490" y1="445" x2="790" y2="320"/>

  <!-- sprinkle stars -->
  <g filter="url(#softGlow)">
    <circle class="nodeDim" cx="95" cy="95" r="2.2"/>
    <circle class="nodeDim" cx="150" cy="210" r="1.8"/>
    <circle class="nodeDim" cx="120" cy="410" r="2.0"/>
    <circle class="nodeDim" cx="880" cy="90" r="2.1"/>
    <circle class="nodeDim" cx="835" cy="235" r="1.7"/>
    <circle class="nodeDim" cx="890" cy="410" r="2.0"/>
    <circle class="nodeDim" cx="420" cy="120" r="1.6"/>
    <circle class="nodeDim" cx="560" cy="110" r="1.6"/>
    <circle class="nodeDim" cx="350" cy="355" r="1.6"/>
    <circle class="nodeDim" cx="625" cy="370" r="1.6"/>
    <circle class="nodeDim" cx="475" cy="505" r="1.4"/>
    <circle class="nodeDim" cx="505" cy="505" r="1.4"/>
  </g>

  <!-- core -->
  <g filter="url(#softGlow)">
    <circle class="nodeCore" cx="490" cy="260" r="7.8"/>
    <text class="label" x="490" y="238" text-anchor="middle">AJ’s question-constellation</text>
    <text class="sublabel" x="490" y="282" text-anchor="middle">clusters I return to when I’m trying to see clearly</text>
  </g>

  <!-- clickable cluster nodes (link to anchors below) -->
  <g filter="url(#softGlow)">
    <!-- Uncertainty -->
    <a href="#uncertainty--belief" class="click">
      <circle class="node" cx="240" cy="145" r="6.2"/>
      <text class="label" x="258" y="150">Uncertainty</text>
      <text class="sublabel" x="258" y="168">beliefs, updating, confidence</text>
    </a>

    <!-- Systems -->
    <a href="#systems--incentives" class="click">
      <circle class="node" cx="185" cy="320" r="6.2"/>
      <text class="label" x="203" y="325">Systems</text>
      <text class="sublabel" x="203" y="343">incentives, scale, failure</text>
    </a>

    <!-- Learning -->
    <a href="#learning--tools" class="click">
      <circle class="node" cx="490" cy="85" r="6.2"/>
      <text class="label" x="508" y="90">Learning</text>
      <text class="sublabel" x="508" y="108">tools, explanation, judgment</text>
    </a>

    <!-- Models -->
    <a href="#models--reality" class="click">
      <circle class="node" cx="745" cy="150" r="6.2"/>
      <text class="label" x="763" y="155">Models</text>
      <text class="sublabel" x="763" y="173">precision, assumptions, truth</text>
    </a>

    <!-- Craft -->
    <a href="#craft--attention" class="click">
      <circle class="node" cx="790" cy="320" r="6.2"/>
      <text class="label" x="808" y="325">Craft</text>
      <text class="sublabel" x="808" y="343">clarity, patience, taste</text>
    </a>

    <!-- Meta -->
    <a href="#meta" class="click">
      <circle class="node" cx="490" cy="445" r="6.2"/>
      <text class="label" x="508" y="450">Meta</text>
      <text class="sublabel" x="508" y="468">language, design of thinking</text>
    </a>
  </g>

  <!-- tiny legend -->
  <text class="tiny" x="60" y="485">tip: click a node to jump to that cluster</text>
</svg>
</div>

---

## Uncertainty & Belief

- When does uncertainty improve judgment rather than degrade it?
- Is confidence more dangerous than ignorance?
- If two people see the same facts and disagree, what is actually different between them?
- Do we update beliefs because of evidence, or because of social permission?

---

## Systems & Incentives

- What breaks first when a system scales: trust, information, or incentives?
- Which systems feel stable only because their failures are slow?
- If no one intends a bad outcome, where does responsibility live?
- How often do systems optimize what’s measurable over what matters?

---

## Learning & Tools

- When does a tool clarify thinking, and when does it replace it?
- Do better tools create better judgment—or just faster mistakes?
- How much understanding disappears behind clean interfaces?
- Is explanation a test of understanding, or a performance?

---

## Models & Reality

- When does a model quietly turn into a belief?
- What do models hide by being precise?
- Are we more afraid of being wrong, or of being wrong publicly?
- How often do we mistake consistency for truth?

---

## Craft & Attention

- What does patience buy that speed cannot?
- When does simplification become distortion?
- How do you tell the difference between elegance and omission?
- What deserves sustained attention in a world optimized for interruption?

---

## Meta

- Which questions keep returning under different disguises?
- How many disagreements are really about language?
- What changes when thinking itself is treated as a design problem?
- Which questions only feel important in retrospect?

---

These questions evolve slowly.  
Some disappear.  
Others refuse to.