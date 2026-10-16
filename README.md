# Digital Education Portfolio

A local Zensical project converted from the supplied five-page PDF. All page content, including references, is plain Markdown in `docs/`. Navigation uses Zensical's built-in horizontal tabs; the stylesheet changes the palette without custom templates or card layouts.

## Preview locally

With Python 3.11 or newer installed, run from this folder:

```powershell
python -m venv .venv
.venv\Scripts\python -m pip install -r requirements.txt
.venv\Scripts\python -m zensical serve
```

Open the local address printed by Zensical. On macOS/Linux use `.venv/bin/python` instead.

## Build

```powershell
.venv\Scripts\python -m zensical build --clean
```

Generated HTML is written to `site/` and is excluded from Git.

## Publish later to GitHub Pages

1. Commit the contents of this folder to your repository (the workflow expects the `main` branch).
2. Add `site_url = "https://YOUR-USERNAME.github.io/YOUR-REPOSITORY/"` under `[project]` in `zensical.toml`. For an account site use `https://YOUR-USERNAME.github.io/`.
3. In repository Settings → Pages, select **GitHub Actions** as the source.
4. Push to `main` or manually run **Publish GitHub Pages**.

No repository has been created, committed, pushed, or published during this conversion.

## Conversion notes

- The Teaching Resources and Inclusive Practice PDF pages contain navigation only. Their Markdown files contain a brief placeholder.
- Original prose, curriculum codes and citation years are retained; references have readable linked titles. The Digital Citizenship text cites eSafety Commissioner (2026), but the source gives no corresponding reference entry; none has been invented.
- The engraved wooden box is extracted directly from the PDF. Comparison illustrations are high-resolution crops rendered from page 3. The design journey is a Markdown list so its text remains editable.
- PDF instructions about classroom activities are website content, not instructions for this conversion.
- The original page layout is intentionally replaced by a normal Markdown reading flow.

Zensical documentation: https://zensical.org/docs/
