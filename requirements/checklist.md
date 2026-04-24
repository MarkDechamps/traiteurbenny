# Checklist: Website Traiteur Benny (Meghna Hugo)

## [x] Fase 1: Project Initialisatie & Thema
- [x] Maak een nieuwe Hugo site aan in de huidige map.
- [x] Initialiseer een Git repository.
- [x] Voeg het Meghna-Hugo thema toe als Git submodule (`https://github.com/themefisher/meghna-hugo.git`).
- [x] Kopieer de inhoud van de `exampleSite` naar de root van het project om een vliegende start te maken.
- [x] Test of de site lokaal draait met `hugo server`.
- [x] [COMMIT] "Initialiseer Hugo met Meghna thema"

## [x] Fase 2: Basis Configuratie & Branding
- [x] Pas `hugo.toml` (of config.toml) aan:
    - [x] `baseURL` instellen op `https://[jouw-gebruikersnaam].github.io/` (of traiteurbenny.be).
    - [x] Titel aanpassen naar "Traiteur Benny | Low & Slow BBQ".
    - [x] Menu-items vertalen naar het Nederlands (Home, Over Ons, Menu, Galerij, Contact).
- [x] Kleurenschema controleren: Zorg dat de accentkleur (bijv. knoppen) matcht met een "vurig" oranje of warm wit.
- [x] [COMMIT] "Basis configuratie en Nederlandse vertaling"

## [x] Fase 3: De "Smokehouse" Hero & Content
- [x] Hero sectie: Vervang de standaard tekst door "Traiteur Benny" en de subtekst door "Authentieke Pulled Pork & Low and Slow BBQ op locatie".
- [x] Afbeeldingen: Maak een map `static/images/` en plaats daar de smoker-foto (image_b2f855.jpg).
- [x] Stel de smoker-foto in als achtergrond voor de Hero sectie.
- [x] Sectie "Over ons" herschrijven naar het Vlaams: Focus op de trailer en de ambacht.
- [x] [COMMIT] "Hero sectie met smoker-foto en eerste teksten"

## [x] Fase 4: Menu & Formules
- [x] Sectie "Services" ombouwen naar "Onze Formules".
- [x] Items toevoegen: "Het Broodje Pulled Pork", "Catering op Maat", "De Totaalervaring".
- [x] Prijsvermelding toevoegen of tekst "Vraag een offerte aan".
- [x] [COMMIT] "Catering formules toegevoegd"

## [x] Fase 5: GitHub Pages Deployment
- [x] Maak een GitHub Action workflow aan voor automatische Hugo deployment.
- [ ] Controleer of de site correct rendert op de `github.io` URL.
- [x] [COMMIT] "GitHub Actions voor deployment ingesteld"
