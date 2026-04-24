# Copilot Instructions — Traiteur Benny

## Project Overview

A multilingual one-page Hugo static site for Traiteur Benny, a Belgian BBQ catering business. Deployed to GitHub Pages at `traiteurbenny.be`.

- **Framework:** Hugo
- **Theme:** [Meghna Hugo](https://github.com/themefisher/meghna-hugo) (added as a Git submodule at `themes/meghna-hugo`)
- **Languages:** NL (default), EN, FR

## Build & Dev Commands

```bash
# Local development server
hugo server

# Build for production
hugo

# Build with drafts
hugo server -D
```

## Architecture

### Multilingual Structure

Content is mirrored across three language folders. **Every content change must be replicated in all three:**

```
content/
  nl/     ← default language (served at traiteurbenny.be/)
  en/     ← served at traiteurbenny.be/en/
  fr/     ← served at traiteurbenny.be/fr/
i18n/     ← string translation files (nl.yaml, en.yaml, fr.yaml)
```

### Hugo Configuration

`hugo.toml` defines `defaultContentLanguage = "nl"` and language blocks for `languages.nl`, `languages.en`, and `languages.fr`, each with their own `languageCode`, `languageName`, `weight`, and menu definitions.

### Theme Integration

The Meghna Hugo theme is a Git submodule. The project's `content/`, `data/`, `assets/`, and `static/` folders at root override the theme's `exampleSite/` equivalents. Do not modify files inside `themes/meghna-hugo/` directly — override them at the root level.

## Key Conventions

- **Strict i18n:** Any content, menu item, or UI string added in `nl/` must have equivalents in `en/` and `fr/`.
- **Commit discipline:** Follow the phased commit messages from `requirements/technical-checklist.md` (e.g., `"T1: ..."`, `"T2: ..."`) and wait for confirmation between phases.
- **Accent color:** BBQ Orange `#e64a19` — used for buttons and primary accents, set via `assets/css/custom.css`.
- **Hero image:** `assets/images/backgrounds/hero-smoker.jpg` — referenced in `data/*/banner.yml`.
- **Contact form:** Handled via Formspree — set the form ID in `data/*/contact.yml`.
- **Deployment:** Automated via `.github/workflows/hugo.yml` targeting GitHub Pages.

## Checklist Tracking

After completing any task listed in `requirements/checklist.md` or `requirements/technical-checklist.md`, **always update the file immediately** by changing `[ ]` to `[x]` for every completed item. Commit the checklist update together with (or directly after) the work commit.

## Implementation Phases

See `requirements/technical-checklist.md` for the full ordered task list. Phases must be completed in sequence:

1. Multilingual scaffold & theme init
2. i18n configuration
3. Visual branding & hero image
4. Content localization
5. Deployment & language switcher
