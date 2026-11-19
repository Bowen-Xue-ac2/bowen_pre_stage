<div align="center">

# Bowen PRE Stage

**Browser-first presentations. One stage, distinct projects.**

[Open US Airlines · Economy](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1) · [Open People & Organisations](https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1) · [Presentation catalogue](#presentations) · [Local preview](#local-preview) · [Credits](#credits-and-licensing)

</div>

---

A public home for interactive presentations, with each deck published under its own URL. This repository hosts the **built website**, separate from the presentation authoring workspace.

## Presentations

| Presentation | Focus | Open |
| --- | --- | --- |
| **People & Organisations · Topic 4** | Servant vs traditional leadership | [Launch presentation](https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1) |
| **US Airlines · Economy** | Short-run costs, price elasticity and oligopoly | [Launch presentation](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1) |

### People & Organisations

**Motion:** “Servant leaders are more effective than traditional leaders.”

A seven-speaker presentation built around leadership practices, fairness, empowerment, teamwork and organisational outcomes. English slide keywords are accompanied by Chinese presenter notes.

- **Visual storytelling** — custom SVG pictograms, staged reveals and animated figures.
- **Web delivery** — interactive slides rather than a video recording.
- **Separate static output** — PDF is a still version; it does not preserve web motion.

This is a working presentation, not a claim that academic review or classroom rehearsal is complete.

### US Airlines · Economy

A 16-slide microeconomics case study of US airline fares, fuel costs, passenger revenue and capacity. The core distinction is **revenue is not profit**: higher fares and premium sales can raise revenue while fuel costs squeeze margins.

- [Open the deck](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1)
- [Source notes](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/sources.html)
- Published files: `economy-pre/`, alongside `ppl-org/`; this is a separate presentation, not a replacement.

#### Current slide map

| Slides | Content |
| --- | --- |
| 1–3 | Opening judgment, Reuters news background and evidence windows, financial results |
| 4–5 | Section E: reported stakeholder outcomes and conditional impacts |
| 6–7 | Short-run costs, including marginal and average total cost |
| 8–9 | PED mechanism and limits of case evidence |
| 10–13 | Oligopoly, limits of kinked demand, scheduled capacity and illustrative game |
| 14 | Conclusion |
| 15–16 | References and list of figures |

#### Source-document coverage review

Rechecked on **18 November 2026** against the **20-slide build at [`9a38286`](https://github.com/Bowen-Xue-ac2/bowen_pre_stage/commit/9a38286)** by inspecting all 20 published slide modules. The four supplied documents, including their embedded figures, were read in the earlier review. **The main gaps identified in the 15-slide build are now addressed.** Coverage means that the substantive teaching points are represented, not that every sentence or original screenshot is reproduced.

| Supplied section | Coverage in current deck | Remaining distinctions |
| --- | --- | --- |
| PED | [8–9](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/8): explicit PED/TR formulas and inelastic range; United's −1.3 pp load factor; occupancy depends on available seats and cannot identify PED without paired fare/volume data; premium-mix caveat. [19](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/19) adds OpenStax §§5.1 and 5.3. | The chart and figures are illustrative, not a numerical estimate of observed airline PED. The label “pp” is used, but percentage points versus percentage changes is not separately explained in prose. |
| Short-run costs | [6–7](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/6) and [18](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/18): short-run/FC/VC definitions; TC, MC, ATC, AVC and AFC formulas; MC/ATC-minimum diagram; contracts, hedges, fleet efficiency, labour and maintenance caveats. | Original schematics replace the source screenshots. The fuel-price rise is not converted into an unsupported equal percentage increase in total cost; the exact total-cost effect is not quantified. |
| Oligopoly | [10–13](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/10): definition, differentiation and entry barriers; four-market-structure comparison; rival responses, kinked demand, capacity and downturn risk; an illustrative payoff matrix. [16](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/16) qualifies inference about intent and coordination. | The game uses newly constructed, explicitly illustrative capacity payoffs rather than reproducing the supplied example. Legal scrutiny is mentioned, but there is no separate antitrust-law explanation or formal price-leadership model. These are narrower than the source, not missing core interdependence analysis. |
| Section E: stakeholders and evaluation | [14–16](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/14): United/rival trade-off, conditional staffing effects, rail/road substitutes, long-route limits, frequency/secondary-airport access, three trade-offs and four limits, including hedges, fleet renewal, endogenous energy prices and the counterfactual. Context remains on 4–5. | Employee and access effects are presented as conditional, not observed outcomes. Welfare losses are not quantified. The source's illustrative fare-times-traffic arithmetic is replaced by a scope/period mismatch warning rather than treated as a valid identity. |

**Remaining review tasks:**

1. Update the separate speaker scripts to the current 20-slide map, especially Section E on **14–16**, the cost exhibit on **18**, and references on **19**. This README update does not modify those documents.
2. If the assessment requires the exact original game, screenshots, explicit antitrust terminology or a percentage-point explanation, confirm those requirements before treating the concise substitutions as equivalent.
3. Check presentation timing and visual readability in rehearsal. This content audit is not a fresh rendered-layout or timing check, nor independent verification of every underlying news claim.

Keep the qualifications in the revised slides: revenue is not profit; premium mix means revenue growth is not necessarily all fare increases; parallel pricing does not establish collusion. Stronger claims in the source drafts about protected margins or proven coordination are intentionally not adopted.

**Historical note:** the [earlier audit at `2078bc6`](https://github.com/Bowen-Xue-ac2/bowen_pre_stage/blob/2078bc69932f134a7d1069111dabb24510fa3338/README.md#source-document-coverage-review) described the **15-slide `27892df` build**. Its missing-item list is superseded by the table above and must not be read as the current status.

This follow-up changes documentation only. It does not change the deck or publish the supplied documents.

## Technology

| Layer | Responsibility |
| --- | --- |
| [Slidev](https://github.com/slidevjs/slidev) | Slide navigation, presentation runtime and presenter notes |
| [Seriph](https://github.com/slidevjs/themes/tree/main/packages/theme-seriph) | Base theme and typography |
| [Vue](https://github.com/vuejs/core) + SVG | Custom visual components and pictogram figures |
| [GSAP](https://github.com/greensock/GSAP) | Figure motion and animation sequencing |
| [Lucide](https://github.com/lucide-icons/lucide) | Interface icons |
| GitHub Pages | Static hosting under project-specific subpaths |

## Repository layout

```text
bowen_pre_stage/
├── README.md
├── .nojekyll
├── economy-pre/
│   ├── index.html          # US Airlines presentation entry
│   ├── assets/             # Compiled application
│   └── sources.html        # Source notes
├── interview/              # Separate published project
└── ppl-org/
    ├── index.html          # Presentation entry
    ├── assets/             # Compiled application
    ├── fonts/              # Locally bundled fonts and notices
    ├── icons/              # SVG icons
    ├── licenses/           # Third-party license texts
    ├── BUILD-INFO.json     # Build and verification record
    └── DEPLOYMENT.md       # Routes and publishing instructions
```

## Local preview

No Node build step is required to preview the published files. With Git and Python 3 installed:

```sh
git clone https://github.com/Bowen-Xue-ac2/bowen_pre_stage.git
python3 -m http.server 8000 --bind 127.0.0.1
```

Run the server from the directory **containing** the cloned repository, then open:

```text
http://localhost:8000/bowen_pre_stage/ppl-org/
http://localhost:8000/bowen_pre_stage/economy-pre/
```

On Windows, use `py -m http.server 8000 --bind 127.0.0.1` if `python3` is unavailable. Serve over HTTP rather than opening `index.html` directly: each build uses its matching `/bowen_pre_stage/<project>/` asset base.

## Publishing model

Each presentation lives in its own directory. To update a deck, build it in its authoring project with the matching base path, then publish the generated files into that directory. Keep other presentation directories and the root README intact.

This repository is a distribution stage, not the complete Slidev source project. Do not edit generated JavaScript bundles as a substitute for updating the source.

## Public content and notes

The repository and presentation are public. **Presenter notes are part of the published client-side content**, including the Chinese notes in this deck. Presenter mode is a viewing mode, not an access-control boundary.

Do not include credentials, private meeting notes or material that should remain restricted.

## Credits and licensing

Third-party software, icons and fonts retain their own licenses. See the bundled [software and icon licenses](ppl-org/licenses/) and [font notices](ppl-org/fonts/COPYRIGHT.txt). GSAP is covered by its [Standard License](ppl-org/licenses/GSAP-STANDARD-LICENSE.txt), not the MIT license.

Public availability does not grant a blanket reuse license for presentation text, artwork or cited third-party material. Consult the relevant notices and original sources before reuse.

README structure inspired by [awesome-readme](https://github.com/matiassingers/awesome-readme): a clear purpose, a direct demo entry, practical usage instructions and explicit credits.
