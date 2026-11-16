<div align="center">

# Bowen PRE Stage

**Browser-first presentations. One stage, distinct projects.**

[Open People & Organisations](https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1) · [Presentation catalogue](#presentations) · [Local preview](#local-preview) · [Credits](#credits-and-licensing)

</div>

---

A public home for interactive presentations, with each deck published under its own URL. This repository hosts the **built website**, separate from the presentation authoring workspace.

## Presentations

| Presentation | Focus | Open |
| --- | --- | --- |
| **People & Organisations · Topic 4** | Servant vs traditional leadership | [Launch presentation](https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1) |

### People & Organisations

**Motion:** “Servant leaders are more effective than traditional leaders.”

A seven-speaker presentation built around leadership practices, fairness, empowerment, teamwork and organisational outcomes. English slide keywords are accompanied by Chinese presenter notes.

- **Visual storytelling** — custom SVG pictograms, staged reveals and animated figures.
- **Web delivery** — interactive slides rather than a video recording.
- **Separate static output** — PDF is a still version; it does not preserve web motion.

This is a working presentation, not a claim that academic review or classroom rehearsal is complete.

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
```

On Windows, use `py -m http.server 8000 --bind 127.0.0.1` if `python3` is unavailable. Serve over HTTP rather than opening `index.html` directly: the build uses the `/bowen_pre_stage/ppl-org/` asset base.

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
