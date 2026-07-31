# AGENTS.md

Turkish MkDocs + Material for MkDocs documentation site (TAMesh, a Meshtastic community project). All content is Turkish — write docs in Turkish, do not translate.

## Verification

- The only check is `mkdocs build --strict` (no tests/lint). Strict mode fails on broken internal links and config warnings. Run it after any change to `mkdocs.yml` or `docs/`.
- Build output goes to `site/` (gitignored) — never commit it.

## Conventions

- **File and directory names are ASCII only** (no Turkish `ı ş ç ğ`): e.g. `yazilim.md` not `yazılım.md`, `baslangic/` not `başlangıç/`. Content is Turkish, paths are ASCII. A `yazılım.md`↔`yazilim.md` mixup already caused missing pages.
- Nav is explicit in `mkdocs.yml` (`nav:`). Under a section, every entry must be a `- list item`; a bare `key: value` line silently drops the section from the sidebar.
- `docs/baslangic/` is a section index page: `baslangic/index.md` is listed as the section's first child *without a title* (relies on the `section-index` plugin) so the "Başlangıç" header links to it without a duplicate sidebar entry. Preserve this pattern for new sections.
- Internal links are relative to the page's directory (e.g. from `docs/baslangic/diy/` to the guide: `../../rehberler/yazilim.md`).
- Use Material admonitions (`!!! note/info/tip/warning/danger`) instead of plain callouts.

## Toolchain gotchas

- Local env: mkdocs 1.6.1, mkdocs-material 9.7.7, mkdocs-section-index 0.3.12.
- **CI mismatch**: `.github/workflows/ci.yml` deploys to GitHub Pages with `mkdocs gh-deploy --force` but only runs `pip install mkdocs-material`. `mkdocs-section-index` is NOT a dependency of `mkdocs-material`, so the deploy breaks if any extra plugin is enabled in `mkdocs.yml`. If you add/keep plugins, add them to the CI `pip install` step (ideally pin versions to match local).
- `mkdocs build --strict` emits a benign "MkDocs may break support for all existing plugins…" warning from an upstream plugin; it is not a config error.
