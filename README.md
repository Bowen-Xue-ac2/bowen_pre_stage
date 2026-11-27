<div align="center">

# Bowen PRE Stage 😊 🤝

**Bowen’s browser-first stage for interactive presentations and product showcases.**

[Schneider Electric](https://bowen-xue-ac2.github.io/bowen_pre_stage/schneider-electric/#/1) · [US Airlines](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1) · [People & Organisations](https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1) · [SILCAI Sandbox](https://bowen-xue-ac2.github.io/bowen_pre_stage/silcai-sandbox/)

[Showcases](#showcases) · [Quick start](#quick-start) · [Build and publish](#build-and-publish) · [Contributing](#contributing) · [Credits](#credits-and-licensing)

</div>

## Showcases

This is the public distribution repository for the built sites. Editable authoring projects live separately.

| Project | What you can explore | Open |
| --- | --- | --- |
| **Schneider Electric · Impact 2030** | A 12-slide social impact assessment with interactive diagrams for energy access and supplier emissions | [Open presentation](https://bowen-xue-ac2.github.io/bowen_pre_stage/schneider-electric/#/1) |
| **People & Organisations · Topic 4** | Servant vs traditional leadership, told with animated visuals and staged reveals | [Launch presentation](https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1) |
| **US Airlines · Economy** | Fuel costs, price elasticity, and how airlines respond to rivals | [Launch presentation](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1) |
| **SILCAI · Product Sandbox** | Rearrange a simulated mobile homepage and try a proposed feature | [Open showcase](https://bowen-xue-ac2.github.io/bowen_pre_stage/silcai-sandbox/) |

### Schneider Electric · Impact 2030

A working group presentation evaluating Schneider Electric’s environmental, social and economic impacts. It follows two theories of change through 2030 and connects the three impact aims to UN Sustainable Development Goals 7, 9 and 13. Selected slides retain editable placeholders for the group’s analysis and references.

- **Browser presentation.** Click the slide or press **→** to advance. Press **←** to go back, including through individual reveals. [Open the interactive deck](https://bowen-xue-ac2.github.io/bowen_pre_stage/schneider-electric/#/1) · [Open the self-contained HTML version](https://bowen-xue-ac2.github.io/bowen_pre_stage/schneider-electric/heartbeat.html#/1)
- **Static PowerPoint.** The 12-slide, 7.46 MB `.pptx` shows each slide fully revealed. Titles, body text, placeholders and diagram labels are editable in PowerPoint. [Download the editable PPTX](schneider-electric/Schneider-Electric-Social-Impact.pptx?raw=true)
- **Authoring and sources.** The source archive includes the Slidev deck and the Mermaid definition. The slide plan records evidence and remaining content slots. [Download the source](schneider-electric/editable-source.zip?raw=true) · [Read the slide plan](schneider-electric/slide-plan.txt) · [View photo credits](schneider-electric/photo-credits.txt)

| Slides | What to look for |
| --- | --- |
| 1–4 | A circuit-board opening, the company mission and three impact aims |
| 5–6 | Slide 5 uses a five-step fishbone diagram to follow energy access from project inputs to the 2030 goal. Slide 6 leaves space for the evaluation. |
| 7–8 | Slide 7 uses six clicks to trace supplier qualification, factory upgrades and proposed emissions verification. The heartbeat moves to the current node. Slide 8 leaves space for the environmental evaluation. |
| 9–12 | Photos illustrate the three UN goals, followed by working layouts for evaluation, conclusion and references |

### SILCAI · Product Sandbox

[Open the showcase](https://bowen-xue-ac2.github.io/bowen_pre_stage/silcai-sandbox/). This is an interactive prototype of the SILCAI mobile homepage for product discussions. It uses simulated data and does not connect to the live mini program.

**Try the current version:** Select **Edit** (编辑), drag the homepage blocks to reorder them, or add **This Week’s To-dos** (本周待办) from the block library. Switch to **Preview** (预览) to open its details and return. Changes stay in this browser across refreshes. **Restore original** (恢复原版) resets the layout. Chat, History, and Profile are placeholders.

**Planned, not yet live:** Create reusable custom blocks, save blocks from the phone back to the library, remove individual blocks from the page, and resize or position blocks freely without forced grid alignment.

Built with Vue 3, TypeScript, Vite, and [Vue.Draggable](https://github.com/SortableJS/vue.draggable.next).

### People & Organisations

**Motion:** “Servant leaders are more effective than traditional leaders.”

A seven-speaker presentation built around leadership practices, fairness, empowerment, teamwork and organisational outcomes. English slide keywords are accompanied by Chinese presenter notes.

- **Visual storytelling** — custom SVG pictograms, staged reveals and animated figures.
- **Web delivery** — interactive slides rather than a video recording.
- **Separate static output** — PDF is a still version; it does not preserve web motion.

This is a working presentation, not a claim that academic review or classroom rehearsal is complete.

### US Airlines · Economy

A 17-slide microeconomics case study of US airline fares, fuel costs, passenger revenue and capacity. The core distinction is **revenue is not profit**: higher fares and premium sales can raise revenue while fuel costs squeeze margins.

- [Open the deck](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1)
- [Source notes](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/sources.html)
- Published files: `economy-pre/`, alongside `ppl-org/`; this is a separate presentation, not a replacement.

#### Current slide map

| Slides | Content |
| --- | --- |
| 1 | Welcome |
| 2 | Reuters case. Click once for United’s leisure load factor and again for Andrew Nocella’s response. |
| 3 | Five-carrier passenger economics with fuel and CPI context |
| 4 | Earnings outlook. Click once to reveal five-carrier Q4 and full-year guidance. |
| 5–6 | Stakeholders and conditional impacts |
| 7–8 | Concept 1: Short-Run Cost — marginal and average total cost |
| 9–10 | Concept 2: Price Elasticity of Demand — mechanism and limits of case evidence |
| 11–13 | Concept 3: Oligopoly — interdependence, kinked demand and capacity choices |
| 14 | Conclusion |
| 15–16 | References |
| 17 | List of figures |

**Evidence and limits.** Passenger revenue is not profit. Premium sales and passenger mix can lift revenue alongside fares; parallel pricing alone does not establish collusion. The [source-document audit](https://github.com/Bowen-Xue-ac2/bowen_pre_stage/blob/cdd90858ca4e831083b245575d1959a0f9fc2f80/README.md#source-document-coverage-review) preserves the earlier 20-slide review. Use the slide map above for the current build.

## Quick start

To browse the published builds locally, use Git and Python 3. No Node build is needed:

```sh
git clone https://github.com/Bowen-Xue-ac2/bowen_pre_stage.git
# Run this from the parent of bowen_pre_stage/
python3 -m http.server 8000 --bind 127.0.0.1
```

Then open:

```text
http://localhost:8000/bowen_pre_stage/schneider-electric/#/1
http://localhost:8000/bowen_pre_stage/ppl-org/
http://localhost:8000/bowen_pre_stage/economy-pre/
http://localhost:8000/bowen_pre_stage/silcai-sandbox/
```

On Windows, use `py -m http.server 8000 --bind 127.0.0.1` if `python3` is unavailable. Serve over HTTP rather than opening `index.html` directly so each project's static assets load correctly.

## Build and publish

1. Make changes in the editable authoring project, not in the generated JavaScript.
2. Build for the matching GitHub Pages project path and replace only that project’s published folder.
3. Verify the page and its assets at the deployed URL. For interactive projects, also test the main flow.

Everything shipped here is public, including client-side presenter notes. Keep credentials, private source or assets, and real student data out of the builds.

### Technology

| Layer | Responsibility |
| --- | --- |
| [Slidev](https://github.com/slidevjs/slidev) | Slide navigation, presentation runtime and presenter notes |
| [Seriph](https://github.com/slidevjs/themes/tree/main/packages/theme-seriph) | Base theme and typography |
| [Vue](https://github.com/vuejs/core) + SVG | Custom visual components and pictogram figures |
| Mermaid | Supplier emissions diagram in the Schneider Electric deck |
| [GSAP](https://github.com/greensock/GSAP) | Figure motion and animation sequencing |
| [Lucide](https://github.com/lucide-icons/lucide) | Interface icons |
| GitHub Pages | Static hosting under project-specific subpaths |

### Repository layout

```text
bowen_pre_stage/
├── README.md
├── DCO
├── .nojekyll
├── economy-pre/
│   ├── index.html          # US Airlines presentation entry
│   ├── assets/             # Compiled application
│   └── sources.html        # Source notes
├── interview/              # Separate published project
├── schneider-electric/
│   ├── index.html          # Interactive Slidev deck
│   ├── heartbeat.html      # Self-contained interactive deck
│   ├── Schneider-Electric-Social-Impact.pptx
│   ├── editable-source.zip
│   ├── slide-plan.txt
│   └── photo-credits.txt
├── silcai-sandbox/         # Compiled mobile product showcase
└── ppl-org/
    ├── index.html          # Presentation entry
    ├── assets/             # Compiled application
    ├── fonts/              # Locally bundled fonts and notices
    ├── icons/              # SVG icons
    ├── licenses/           # Third-party license texts
    ├── BUILD-INFO.json     # Build and verification record
    └── DEPLOYMENT.md       # Routes and publishing instructions
```

## Contributing

Open an issue for a proposal or submit a focused PR. Name the affected showcase, describe the change, and include a preview or what you tested.

### DCO sign-off

Read the [Developer Certificate of Origin 1.1](DCO) and sign off each of your own contributions if you can make that certification:

```sh
git commit --signoff -m "Describe the change"
```

Git adds a `Signed-off-by:` trailer from your configured name and email. This certifies your right to submit the contribution; it is not a cryptographic signature and does not substitute for a license. Your sign-off is part of the public commit history. Do not sign off on someone else’s behalf.

## Credits and licensing

Third-party software, icons and fonts retain their own licenses. See the bundled [software and icon licenses](ppl-org/licenses/) and [font notices](ppl-org/fonts/COPYRIGHT.txt). GSAP is covered by its [Standard License](ppl-org/licenses/GSAP-STANDARD-LICENSE.txt), not the MIT license.

Public availability does not grant a blanket reuse license for presentation text, artwork or cited third-party material. Consult the relevant notices and original sources before reuse.

README structure inspired by [awesome-readme](https://github.com/matiassingers/awesome-readme): a clear purpose, a direct demo entry, practical usage instructions and explicit credits.
