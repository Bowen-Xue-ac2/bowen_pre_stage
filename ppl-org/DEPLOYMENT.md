# GitHub Pages handoff — Topic 4 pictogram

Extract the CONTENTS of this ZIP directly into the repository's `ppl-org/` directory. Do not add another `dist/` or `ppl-org/` nesting level. The ZIP root contains index.html, assets/, fonts/, icons/, licenses/ and favicon.svg. Keep a .nojekyll file at the repository root for prebuilt static publishing; the enclosed empty .nojekyll may also be copied there.

Repository: Bowen-Xue-ac2/bowen_pre_stage. Pages source: main / root.
Base: /bowen_pre_stage/ppl-org/
Router: hash. No SPA rewrite, _redirects, server runtime or build service is needed.

After deployment, the expected URLs are:
- https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/1
- https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/4?clicks=2
- https://bowen-xue-ac2.github.io/bowen_pre_stage/ppl-org/#/presenter/7

Use hash routes rather than /ppl-org/4. Click state belongs after the hash, as shown above. For Slidev's print mode use /ppl-org/?print=true#/6 (print is before the hash).

Chinese presenter notes are retained in the compiled application, as explicitly requested for public publication. Fonts, icons, framework scripts and all included licenses are local. Keep the licenses/ and fonts/COPYRIGHT.txt files. No CDN is required.

Source content, citations, Chinese notes, pictogram geometry and styling were preserved. The only scene-controller adjustment sets p07 bubble y to zero during SPA navigation, eliminating an inherited 12px entrance shift; all 24 final screenshots match the verified original exactly. No PDF, screenshots, source Notion snapshot, node_modules or private Beauty repository files are in this ZIP.

Validation was run in Beauty against an ordinary static server at the exact nested prefix, with NO SPA fallback. Hash deep links and refresh, presenter notes, embedded fonts, resources, motion interruptions/back/re-entry/reduced-motion and mouse-to-keyboard navigation passed. See BUILD-INFO.json. The real GitHub Pages URL and real iOS have not been tested by this packaging task.

Build command in the isolated adapter source:
    slidev build slides.md --out dist --base /bowen_pre_stage/ppl-org/ --router-mode hash
Notes were not stripped. Original font bytes match Beauty's installed Liberation font files.

Integrity check from this extracted directory:
    sha256sum -c SHA256SUMS.txt
The build digest reported to the parent is SHA256(SHA256SUMS.txt), whose UTF-8 lines are sorted by relative POSIX file path, formatted as SHA256 + two spaces + path + LF. It covers every packaged file except the checksum file itself.
