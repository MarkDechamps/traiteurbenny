Project Specification: Traiteur Benny (Multilingual)
Goal: A multilingual (NL, EN, FR) one-page Hugo site.
Tech Stack: Hugo, Meghna Hugo Theme, GitHub Pages.
Languages: - NL (Default): traiteurbenny.be/

EN: traiteurbenny.be/en/

FR: traiteurbenny.be/fr/

Technical Checklist for Copilot
[x] Phase 1: Multilingual Environment Setup
[x] Initialize Hugo: Run hugo new site . --force and git init.

[x] Theme Integration: Add Meghna Hugo as a submodule: git submodule add https://github.com/themefisher/meghna-hugo.git themes/meghna-hugo.

[x] Multilingual Scaffold:

[x] Create content/nl/, content/en/, and content/fr/ directories.

[x] Copy themes/meghna-hugo/exampleSite/content/* into all three language folders.

[x] Copy the data/ and assets/ folders from exampleSite to the root.

[x] [COMMIT] "T1: Multilingual scaffold and theme initialized"

[x] Phase 2: Multilingual Configuration
[x] Configure hugo.toml for i18n:

[x] Define languages.nl, languages.en, and languages.fr.

[x] Set defaultContentLanguage = "nl".

[x] Enable languageCode, languageName, and weight for each language.

[x] Navigation Translation: Define localized menus in the config for all three languages (Home, About, Menu, Contact).

[x] [COMMIT] "T2: i18n configuration for NL, EN, and FR completed"

[x] Phase 3: Visual Branding & Assets
[x] Hero Asset: Place the smoker image in static/images/hero-smoker.jpg.

[x] Hero Integration: Update the homepage content files (e.g., content/nl/_index.md, etc.) to use /images/hero-smoker.jpg as the background.

[x] Style Tweak: Set primary accent color to BBQ Orange (#e64a19) in the theme's SCSS variables or custom CSS.

[x] [COMMIT] "T3: Visual branding and smoker hero image integrated"

[x] Phase 4: Content Localization (Baby Steps)
[x] Dutch (NL): Set core text: "Traiteur Benny - Low & Slow BBQ".

[x] English (EN): Set core text: "Catering Benny - Authentic BBQ & Smoker".

[x] French (FR): Set core text: "Traiteur Benny - BBQ Authentique & Fumoir".

[x] [COMMIT] "T4: Core homepage headlines localized in 3 languages"

[x] Phase 5: Deployment & Forms
[x] Language Switcher: Ensure the theme's language switcher is enabled in the navigation bar.

[x] Contact Form: Set up a multilingual-ready contact form using a service like Formspree.

[x] GitHub Action: Create .github/workflows/hugo.yml for automated deployment.

[x] [COMMIT] "T5: Deployment workflow and language switcher active"

Instructions for Copilot:
Strict i18n: Ensure that every content change is mirrored across the nl/, en/, and fr/ folders.

ExampleSite Copy: When copying the exampleSite, make sure to move the i18n/ folder (if present) to the root to manage string translations.

One Step at a Time: Perform the tasks in order and wait for confirmation after each [COMMIT] point.
