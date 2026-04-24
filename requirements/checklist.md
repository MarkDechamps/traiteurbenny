# Checklist: Website Traiteur Benny (Meghna Hugo)

## [ ] Fase 1: Project Initialisatie & Thema
- [ ] Maak een nieuwe Hugo site aan in de huidige map.
- [ ] Initialiseer een Git repository.
- [ ] Voeg het Meghna-Hugo thema toe als Git submodule (`https://github.com/themefisher/meghna-hugo.git`).
- [ ] Kopieer de inhoud van de `exampleSite` naar de root van het project om een vliegende start te maken.
- [ ] Test of de site lokaal draait met `hugo server`.
- [ ] [COMMIT] "Initialiseer Hugo met Meghna thema"

## [ ] Fase 2: Basis Configuratie & Branding
- [ ] Pas `hugo.toml` (of config.toml) aan:
    - [ ] `baseURL` instellen op `https://[jouw-gebruikersnaam].github.io/` (of traiteurbenny.be).
    - [ ] Titel aanpassen naar "Traiteur Benny | Low & Slow BBQ".
    - [ ] Menu-items vertalen naar het Nederlands (Home, Over Ons, Menu, Galerij, Contact).
- [ ] Kleurenschema controleren: Zorg dat de accentkleur (bijv. knoppen) matcht met een "vurig" oranje of warm wit.
- [ ] [COMMIT] "Basis configuratie en Nederlandse vertaling"

## [ ] Fase 3: De "Smokehouse" Hero & Content
- [ ] Hero sectie: Vervang de standaard tekst door "Traiteur Benny" en de subtekst door "Authentieke Pulled Pork & Low and Slow BBQ op locatie".
- [ ] Afbeeldingen: Maak een map `static/images/` en plaats daar de smoker-foto (image_b2f855.jpg).
- [ ] Stel de smoker-foto in als achtergrond voor de Hero sectie.
- [ ] Sectie "Over ons" herschrijven naar het Vlaams: Focus op de trailer en de ambacht.
- [ ] [COMMIT] "Hero sectie met smoker-foto en eerste teksten"

## [ ] Fase 4: Menu & Formules
- [ ] Sectie "Services" ombouwen naar "Onze Formules".
- [ ] Items toevoegen: "Het Broodje Pulled Pork", "Catering op Maat", "De Totaalervaring".
- [ ] Prijsvermelding toevoegen of tekst "Vraag een offerte aan".
- [ ] [COMMIT] "Catering formules toegevoegd"

## [ ] Fase 5: GitHub Pages Deployment
- [ ] Maak een GitHub Action workflow aan voor automatische Hugo deployment.
- [ ] Controleer of de site correct rendert op de `github.io` URL.
- [ ] [COMMIT] "GitHub Actions voor deployment ingesteld"
