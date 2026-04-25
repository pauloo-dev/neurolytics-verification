# QualSight — Interactive Qualitative Analysis Tool

> **Beyond the Blueprint: Exploring Teachers' Adaptive Agency in Maximising Inclusive Utility under Kenya's CBC**
>
---



## 🎓 Research Context

| Field | Detail |
|---|---|
| **Programme** | MSc Education |
| **Institution** | School of Education |
| **Dissertation title** | *Beyond the Blueprint: Exploring Teachers' Adaptive Agency in Maximising Inclusive Utility under Kenya's CBC* |
| **Study site** | Nakuru County, Kenya — urban, peri-urban & rural public primary schools |
| **Participants** | n = 9 teachers (7 mainstream · 1 SNE specialist · 1 mixed) |
| **Data** | ~9 hours of semi-structured interview audio; verbatim transcripts |
| **Methodology** | Qualitative interviews-only; reflexive thematic analysis (Braun & Clarke, 2006); abductive orientation |
| **Epistemology** | Social constructivism |
| **Axiology** | Social justice / equity |

### Research Questions

**RQ1** — How do teachers perceive and enact inclusive practices to maximise inclusive utility (presence, participation, progression) for neurodivergent learners in CBC classrooms?

**RQ2** — What adaptive strategies and institutional conditions enable or constrain teachers' efforts to maximise inclusive utility under CBC in Kenyan public primary schools?

### Theoretical Frameworks

- **Universal Design for Learning (UDL)** — Meyer, Rose & Gordon (2014)
- **Ecological Systems Theory** — Bronfenbrenner (1979); reconceptualised by Anderson, Boyle & Deppeler (2014)
- **Value-Based Education (VBE) & DisCrit** — Ngwacho (2024); Annamma, Connor & Ferri (2012)
- **Social Constructivism** — Vygotsky (1978)
- **Inclusive Utility (3P)** — original conceptual construct developed in this study; operationalises Presence, Participation & Progression as a decision lens for teachers assembling *adaptation ensembles*

---

## ✨ Features

### 📊 Dashboard
- Study metadata, RQ display, and methodological framework at a glance
- Stat cards: participants, themes, codes, interview duration
- Interactive Chart.js visualisations — theme frequency bar chart & school context doughnut
- Full participant summary table with context, grade level, class size, experience, and SEN profile
- Sensitising lens reference panel with positionality note

### 🎯 Themes & Quotes
Seven reflexively generated themes, each with:
- Full narrative description with embedded theoretical signposting
- Colour-coded sensitising lens labels
- Code pill cloud
- Expandable representative quote panels (50+ quotes total, sourced and attributed)

| # | Theme |
|---|---|
| T1 | Adaptation Ensembles: Assembling the Feasible Frontier |
| T2 | Inclusive Utility in Practice: Reading the 3Ps |
| T3 | Structural-Ecological Tensions: The Borrowed Architecture Problem |
| T4 | Lateral Collaboration as Lifeline: Cooperation Without Infrastructure |
| T5 | Teacher Adaptive Agency as Moral Vocation |
| T6 | Neurodivergence: Between Recognition, Resourcelessness, and the Strength-Turn |
| T7 | The CBE Paradox: Aspirational Design, Enacted Contradiction |

### 📖 Codebook
- 34 codes across 7 parent categories
- Each code includes: name (in `CATEGORY :: snake_case` format), definition, analytical note, and a frequency bar showing how many of the 9 participants the code appears in
- Categories: Adaptation Ensembles · Inclusive Utility (3P) · Structural-Ecological Conditions · Collaboration · Teacher Agency & Moral Vocation · Neurodivergence Recognition · CBE Paradox

### ⊞ Participant × Theme Matrix
- 9 × 7 cross-tabulation of theme engagement depth: ● High · ◑ Medium · ○ Low
- Radar chart comparing theme coverage by school context (Urban / Rural / SNE)
- Four embedded analytic memos on cross-cutting matrix patterns

### ◐ Thematic Map
- SVG diagram showing directional relationships between all 7 themes and the central construct of *Inclusive Utility (3P)*
- RQ-to-theme routing clearly annotated
- Enabling and constraining relationships distinguished
- Theoretical integration note explaining the conceptual architecture

### ⌕ Search & Filter
- Live keyword search across all 50+ representative quotes
- Filter by participant ID (T01–T09)
- Filter by theme (T1–T7)
- Combined filtering with real-time result count and keyword highlighting

---


## 🛠️ Technical Stack

| Layer | Technology |
|---|---|
| **Markup** | Semantic HTML5 |
| **Styling** | Vanilla CSS3 — CSS custom properties, `clamp()`, CSS Grid, Flexbox, responsive `@media` queries |
| **Charts** | [Chart.js 4.4.1](https://www.chartjs.org/) via cdnjs CDN |
| **Diagrams** | Inline SVG with `<marker>` arrowheads and `<filter>` glow effects |
| **Typography** | Google Fonts — Playfair Display (display) · IBM Plex Sans (body) · IBM Plex Mono (code/IDs) |
| **Interactivity** | Vanilla JavaScript — no frameworks, no build tools |
| **Distribution** | Single self-contained `.html` file (~140KB) |


---

## 🚀 Usage

### Embed in a portfolio or research site
```html
<iframe src="qualsight_responsive.html" width="100%" height="800px" style="border:none;border-radius:8px"></iframe>
```

### Fork and adapt for your own qualitative project
The quote database is a plain JavaScript array at the bottom of the file:

```javascript
const allQuotes = [
  {
    pid: 'T01',         // participant ID — drives pill colour
    theme: 'T1',        // maps to themeNames and themeColors
    codes: ['Heterogeneous grouping', 'Seating'],
    text: 'The grouping is heterogeneous...',
    ctx: 'On differentiated teaching methodologies'  // optional
  },
  // ...
];
```

To adapt for a new project, update:
1. `allQuotes` — your own coded quotes
2. `themeNames` and `themeColors` — your theme labels and colours
3. The theme card markup in `#panel-themes`
4. The codebook markup in `#panel-codebook`
5. The matrix table in `#panel-matrix`
6. Chart data arrays in the `window.addEventListener('load', ...)` block

---

## 📁 Repository Structure

```
qualsight/
│
├── qualsight_responsive.html   # ← Main application (self-contained)
└── README.md                   # ← This file
```

## 🔬 Key Findings (Summary)

Seven themes were generated from nine semi-structured interviews with teachers across urban, peri-urban, and rural public primary schools in Nakuru County, Kenya:

1. **Adaptation Ensembles** — Teachers assemble context-specific bundles of low-cost adjustments (heterogeneous grouping, translanguaging, visual mediation, peer pairing, flexible pacing) calibrated to what is feasible within structural constraints. These are not policy-mandated but emerge from situated pedagogical judgement.

2. **Inclusive Utility (3P)** — All nine participants demonstrate a working awareness of Presence, Participation, and Progression, even without the terminology. Progression is primarily measured through small observable wins rather than test scores — a de facto alignment with CBE's competency logic.

3. **Structural-Ecological Tensions** — Kenya's CBE was modelled on Nordic systems assuming tripartite support, small classes, and universal assistive technology — none of which are present. Class sizes reach 90. Government tablets are non-functional. Teachers fund digital resources personally.

4. **Lateral Collaboration** — In the absence of vertical support structures, WhatsApp groups serve as de facto professional infrastructure. What is described is largely *cooperation* rather than true *collaboration* — the structures lack joint problem-solving, role clarity, and reciprocal accountability.

5. **Moral Vocation** — Adaptation for inclusion is framed universally as moral calling ("ni moyo"). This sustains adaptive practice under severe constraint but also masks structural deficits and is not scalable.

6. **Neurodivergence Recognition** — All participants describe learners with features of autism, ADHD, dyslexia, and sensorimotor difficulties — yet almost none have formal diagnostic support. A spontaneous strength-based turn is visible across participants, prefiguring the neurodiversity paradigm's core claim.

7. **The CBE Paradox** — Teachers endorse CBE's inclusive aspirations while documenting a persistent implementation gap. Examination pressure, content overload, and merit-based stratification persist inside a system publicly disavowing them. The pathway system is good policy encountered as non-functioning in practice.

---

## 📚 Key References

- Annamma, S. A., Connor, D., & Ferri, B. (2012). Disability Critical Race Theory (*DisCrit*). *Race Ethnicity and Education, 16*(1), 1–31.
- Armstrong, T. (2012). *Neurodiversity in the classroom*. ASCD.
- Braun, V., & Clarke, V. (2006). Using thematic analysis in psychology. *Qualitative Research in Psychology, 3*(2), 77–101.
- Bronfenbrenner, U. (1979). *The ecology of human development*. Harvard University Press.
- Florian, L. (2014). What counts as evidence of inclusive education? *European Journal of Special Needs Education, 29*(3), 286–294.
- Meyer, A., Rose, D. H., & Gordon, D. (2014). *Universal design for learning: Theory and practice*. CAST.
- Mulholland, M., & O'Connor, U. (2016). Collaborative classroom practice for inclusion. *International Journal of Inclusive Education, 20*(10), 1070–1083.
- Ngwacho, G. A. (2024). Value-based education incorporation in CBC. *Journal of the Kenya National Commission for UNESCO, 4*(1).
- Phillips, D., & Ochs, K. (2003). Processes of policy borrowing in education. *Comparative Education, 39*(4), 451–461.
- Vygotsky, L. S. (1978). *Mind in society*. Harvard University Press.
- Volmari, K. (Ed.) (2019). *Basic education in the Nordic region*. Finnish National Agency for Education.

---


## 📄 Licence

The **code** (HTML/CSS/JS) in this repository is released under the [MIT Licence](LICENSE) — you are free to fork, adapt, and redistribute it for your own qualitative research projects.

The **research data, quotes, analysis, and written content** remain the intellectual property of Beatrice Wairimu Mungai and the University of Glasgow. They may not be reproduced, cited, or published without explicit permission from the author and appropriate academic attribution.

---

<div align="center">
</div>
