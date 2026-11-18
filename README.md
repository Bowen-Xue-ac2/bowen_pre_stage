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

A 20-slide microeconomics case study of US airline fares, fuel costs, passenger revenue and capacity. The core distinction is **revenue is not profit**: higher fares and premium sales can raise revenue while fuel costs squeeze margins.

- [Open the deck](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/1)
- [Source notes](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/sources.html)
- Published files: `economy-pre/`, alongside `ppl-org/`; this is a separate presentation, not a replacement.

#### Current slide map

| Slides | Content |
| --- | --- |
| 1–3 | Executive summary, industry data and revenue versus profit |
| 4–5 | Stakeholders: airlines, passengers and fuel suppliers |
| 6–7 | Short-run costs, marginal cost and average-cost relationships |
| 8–9 | Price elasticity of demand and limits of the available evidence |
| 10–11 | Route-level oligopoly and the kinked-demand model |
| 12–13 | Capacity outlook and illustrative strategic game |
| 14–16 | Section E: carriers and rivals, passengers, trade-offs and limits |
| 17–18 | Conclusion and short-run cost exhibit |
| 19–20 | References and list of figures |

#### Source-document coverage review

Reviewed on **18 November 2026** against the 15-slide published build at [`27892df`](https://github.com/Bowen-Xue-ac2/bowen_pre_stage/commit/27892dfb8dff088a9db02358e688dba83425545a), cross-checked with its PDF export. All four supplied documents were read, including embedded figures. **Core arguments are present, but none of the four documents is reproduced in full.** This is a content-coverage check, not independent verification of every underlying news claim.

| Supplied section | Coverage in current deck | Still absent or only implicit |
| --- | --- | --- |
| PED | [8–9](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/8), with industry evidence on 2–3: inelastic-demand revenue example, premium mix and incompatible data periods | Explicit `PED = %ΔQd / %ΔP`, `abs(PED) < 1` and `TR = P × Q` notation; United's 1.3-percentage-point load-factor example and the distinction between load factor and quantity; supplied OpenStax references |
| Short-run costs | [6–7](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/6), fuel data on 2: MC/AVC/ATC effects, unchanged AFC at fixed output, `AFC = FC / Q` and `ATC = AFC + AVC` | Formal short-run/FC/VC definitions; `TC = FC + VC`, `MC = ΔTC / ΔQ`, `ATC = TC / Q`, `AVC = VC / Q`; the supplied MC/ATC-minimum diagram; explicit labour, maintenance and contract/hedging caveats. The current deck instead uses an MC-shift figure and mentions purchase price/fuel burn. |
| Oligopoly | [10–12](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/10): route competition, entry barriers, rival responses, kinked demand and capacity | Compact definition including product differentiation; supplied market-structure comparison and game-theory payoff example; explicit antitrust and recession caveats. The deck reframes the source around route-level evidence rather than treating similar price moves as collusion. |
| Section E: stakeholders and evaluation | [4–5](https://bowen-xue-ac2.github.io/bowen_pre_stage/economy-pre/#/4), with related analysis across 6–13: affordability, airline margins, measurement limits and no inference of agreement | Employees are not covered despite the source's cross-reference; rail/road substitutes and long-haul limits; frequency/secondary-airport access; the explicit three-tradeoff/four-limit structure; hedging, fleet renewal, endogenous input prices and the defensive-versus-opportunistic counterfactual. United's load-factor example is also absent. |

**Before calling the deck fully aligned:**

1. Add the missing PED notation and, if retained after source checking, the United example with the percentage-point/load-factor caveat.
2. Add a compact cost-definition/formula block. Decide whether the additional source diagram is needed rather than duplicating theory.
3. Resolve Section E's missing stakeholder and evaluation points, and update all script slide numbers to the current 15-slide map. Source references to “slides 7–9” or “9–11” no longer identify the same sections.
4. Reconcile references, including OpenStax if its material is incorporated.

Do not import unsupported stronger claims from the drafts: rising revenue does not establish protected margins; premium mix means revenue growth is not necessarily all fare increases; parallel pricing does not establish collusion. Missing source content is a review item, not automatic approval to add it.

This review updates documentation only. It does not change the deck, publish the supplied documents or certify the slides as complete.

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
