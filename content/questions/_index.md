---
title: "Questions"
aliases: /questions
description: "Thought experiments I think with"
---

“The true delight is in the finding out rather than in the knowing.”  
<small>— Isaac Asimov</small>

---

{{< rawhtml >}}
<div class="constellation-map" style="max-width: 980px; margin: 2rem auto;">
<svg viewBox="0 0 980 560" width="100%" height="auto" role="img" aria-label="A constellation map of question clusters and recurring motifs">
  <defs>
    <filter id="softGlow" x="-30%" y="-30%" width="160%" height="160%">
      <feGaussianBlur stdDeviation="2.1" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>
    <style>
      .constellation-bg { fill: transparent; }
      .constellation-skyline { stroke: currentColor; stroke-width: 1.25; opacity: 0.1; }
      .constellation-link { stroke: currentColor; stroke-width: 1.2; opacity: 0.2; }
      .constellation-link2 { stroke: currentColor; stroke-width: 1.0; stroke-dasharray: 3 6; opacity: 0.15; }
      .constellation-motifLink { stroke: currentColor; stroke-width: 1.0; opacity: 0.15; }
      .constellation-motifLink2 { stroke: currentColor; stroke-width: 0.95; stroke-dasharray: 2.5 7; opacity: 0.1; }
      .constellation-node { fill: currentColor; opacity: 0.9; }
      .constellation-nodeDim { fill: currentColor; opacity: 0.4; }
      .constellation-nodeCore { fill: currentColor; opacity: 0.95; }
      .constellation-motif { fill: currentColor; opacity: 0.6; }
      .constellation-label { fill: currentColor; font: 600 15px 'Inter', ui-sans-serif, system-ui, sans-serif; letter-spacing: 0.2px; opacity: 0.9; }
      .constellation-sublabel { fill: currentColor; font: 500 12.5px 'Inter', ui-sans-serif, system-ui, sans-serif; opacity: 0.5; }
      .constellation-tiny { fill: currentColor; font: 500 11px 'Inter', ui-sans-serif, system-ui, sans-serif; opacity: 0.35; }
      .constellation-motifLabel { fill: currentColor; font: 600 11.5px 'Inter', ui-sans-serif, system-ui, sans-serif; letter-spacing: 0.2px; opacity: 0.45; }
      .constellation-ring { fill: none; stroke: currentColor; stroke-width: 1.0; opacity: 0.1; }
      .constellation-click { cursor: pointer; }
      .constellation-click:hover .constellation-node { opacity: 1; }
      .constellation-click:hover .constellation-label { opacity: 1; }
    </style>
  </defs>
  <rect class="constellation-bg" x="0" y="0" width="980" height="560"/>
  <line class="constellation-skyline" x1="60" y1="495" x2="920" y2="495"/>
  <circle class="constellation-ring" cx="490" cy="285" r="88"/>
  <circle class="constellation-ring" cx="490" cy="285" r="155"/>
  <circle class="constellation-ring" cx="490" cy="285" r="225"/>
  <line class="constellation-link" x1="490" y1="285" x2="240" y2="165"/>
  <line class="constellation-link" x1="490" y1="285" x2="745" y2="170"/>
  <line class="constellation-link" x1="490" y1="285" x2="185" y2="345"/>
  <line class="constellation-link" x1="490" y1="285" x2="790" y2="345"/>
  <line class="constellation-link" x1="490" y1="285" x2="490" y2="100"/>
  <line class="constellation-link" x1="490" y1="285" x2="490" y2="475"/>
  <line class="constellation-link2" x1="240" y1="165" x2="185" y2="345"/>
  <line class="constellation-link2" x1="745" y1="170" x2="790" y2="345"/>
  <line class="constellation-link2" x1="490" y1="100" x2="745" y2="170"/>
  <line class="constellation-link2" x1="490" y1="100" x2="240" y2="165"/>
  <line class="constellation-link2" x1="490" y1="475" x2="185" y2="345"/>
  <line class="constellation-link2" x1="490" y1="475" x2="790" y2="345"/>
  <g filter="url(#softGlow)">
    <circle class="constellation-nodeDim" cx="95" cy="105" r="2.2"/>
    <circle class="constellation-nodeDim" cx="150" cy="230" r="1.8"/>
    <circle class="constellation-nodeDim" cx="120" cy="440" r="2.0"/>
    <circle class="constellation-nodeDim" cx="880" cy="105" r="2.1"/>
    <circle class="constellation-nodeDim" cx="835" cy="255" r="1.7"/>
    <circle class="constellation-nodeDim" cx="890" cy="440" r="2.0"/>
    <circle class="constellation-nodeDim" cx="420" cy="135" r="1.6"/>
    <circle class="constellation-nodeDim" cx="560" cy="125" r="1.6"/>
    <circle class="constellation-nodeDim" cx="350" cy="385" r="1.6"/>
    <circle class="constellation-nodeDim" cx="625" cy="400" r="1.6"/>
    <circle class="constellation-nodeDim" cx="475" cy="545" r="1.4"/>
    <circle class="constellation-nodeDim" cx="505" cy="545" r="1.4"/>
  </g>
  <g filter="url(#softGlow)">
    <circle class="constellation-nodeCore" cx="490" cy="285" r="8.0"/>
    <text class="constellation-label" x="490" y="258" text-anchor="middle">AJ's question-constellation</text>
    <text class="constellation-sublabel" x="490" y="306" text-anchor="middle">clusters + recurring motifs I use to see more clearly</text>
  </g>
  <g filter="url(#softGlow)">
    <a href="#uncertainty--belief" class="constellation-click"><circle class="constellation-node" cx="240" cy="165" r="6.4"/><text class="constellation-label" x="258" y="170">Uncertainty</text><text class="constellation-sublabel" x="258" y="188">beliefs, updating, confidence</text></a>
    <a href="#systems--incentives" class="constellation-click"><circle class="constellation-node" cx="185" cy="345" r="6.4"/><text class="constellation-label" x="203" y="350">Systems</text><text class="constellation-sublabel" x="203" y="368">incentives, scale, failure</text></a>
    <a href="#learning--tools" class="constellation-click"><circle class="constellation-node" cx="490" cy="100" r="6.4"/><text class="constellation-label" x="508" y="105">Learning</text><text class="constellation-sublabel" x="508" y="123">tools, explanation, judgment</text></a>
    <a href="#models--reality" class="constellation-click"><circle class="constellation-node" cx="745" cy="170" r="6.4"/><text class="constellation-label" x="763" y="175">Models</text><text class="constellation-sublabel" x="763" y="193">assumptions, truth, precision</text></a>
    <a href="#craft--attention" class="constellation-click"><circle class="constellation-node" cx="790" cy="345" r="6.4"/><text class="constellation-label" x="808" y="350">Craft</text><text class="constellation-sublabel" x="808" y="368">clarity, patience, taste</text></a>
    <a href="#meta" class="constellation-click"><circle class="constellation-node" cx="490" cy="475" r="6.4"/><text class="constellation-label" x="508" y="480">Meta</text><text class="constellation-sublabel" x="508" y="498">language, design of thinking</text></a>
  </g>
  <g filter="url(#softGlow)">
    <circle class="constellation-motif" cx="690" cy="120" r="3.2"/><text class="constellation-motifLabel" x="702" y="124">attention</text>
    <circle class="constellation-motif" cx="570" cy="150" r="3.2"/><text class="constellation-motifLabel" x="582" y="154">intuition</text>
    <circle class="constellation-motif" cx="280" cy="380" r="3.2"/><text class="constellation-motifLabel" x="292" y="384">misalignment</text>
    <circle class="constellation-motif" cx="310" cy="250" r="3.2"/><text class="constellation-motifLabel" x="322" y="254">automation</text>
    <circle class="constellation-motif" cx="700" cy="410" r="3.2"/><text class="constellation-motifLabel" x="712" y="414">overfitting</text>
    <circle class="constellation-motif" cx="610" cy="470" r="3.2"/><text class="constellation-motifLabel" x="622" y="474">legibility</text>
    <circle class="constellation-motif" cx="410" cy="140" r="3.2"/><text class="constellation-motifLabel" x="422" y="144">fragility</text>
    <circle class="constellation-motif" cx="265" cy="120" r="3.2"/><text class="constellation-motifLabel" x="277" y="124">narrative</text>
  </g>
  <line class="constellation-motifLink" x1="690" y1="120" x2="790" y2="345"/>
  <line class="constellation-motifLink2" x1="690" y1="120" x2="490" y2="100"/>
  <line class="constellation-motifLink2" x1="690" y1="120" x2="745" y2="170"/>
  <line class="constellation-motifLink2" x1="570" y1="150" x2="240" y2="165"/>
  <line class="constellation-motifLink" x1="570" y1="150" x2="490" y2="100"/>
  <line class="constellation-motifLink2" x1="570" y1="150" x2="745" y2="170"/>
  <line class="constellation-motifLink" x1="280" y1="380" x2="185" y2="345"/>
  <line class="constellation-motifLink2" x1="280" y1="380" x2="745" y2="170"/>
  <line class="constellation-motifLink" x1="310" y1="250" x2="185" y2="345"/>
  <line class="constellation-motifLink2" x1="310" y1="250" x2="490" y2="100"/>
  <line class="constellation-motifLink" x1="700" y1="410" x2="745" y2="170"/>
  <line class="constellation-motifLink2" x1="700" y1="410" x2="490" y2="475"/>
  <line class="constellation-motifLink" x1="610" y1="470" x2="790" y2="345"/>
  <line class="constellation-motifLink2" x1="610" y1="470" x2="490" y2="475"/>
  <line class="constellation-motifLink" x1="410" y1="140" x2="240" y2="165"/>
  <line class="constellation-motifLink2" x1="410" y1="140" x2="745" y2="170"/>
  <line class="constellation-motifLink2" x1="265" y1="120" x2="240" y2="165"/>
  <line class="constellation-motifLink" x1="265" y1="120" x2="185" y2="345"/>
  <text class="constellation-tiny" x="60" y="525">tip: click a major node to jump to that cluster</text>
  <text class="constellation-tiny" x="60" y="545">small satellites are recurring motifs (not categories)</text>
</svg>
</div>
{{< /rawhtml >}}

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