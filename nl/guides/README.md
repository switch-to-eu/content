# Documentatie voor Gidsbijdragers

Welkom bij de Switch-to.EU gidsdocumentatie! Deze README biedt alles wat je moet weten over het maken en onderhouden van migratiegidsen voor EU-servicealternatieven.

## Gidsstructuur

Elke migratiegids moet in de juiste categoriemap worden geplaatst en deze structuur volgen:

```
/content/guides/[categorie]/[service-naam]/
├── index.mdx          # De hoofdinhoud van de gids
└── images/            # Afbeeldingenmap voor screenshots en diagrammen
    ├── step1.png
    ├── step2.png
    └── ...
```

## Gidscategorieën

Gidsen zijn georganiseerd per servicecategorie:

- `email` - E-maildiensten
- `storage` - Cloudopslagdiensten
- `messaging` - Chat- en berichtentoepassingen
- `productivity` - Kantoor- en productiviteitstools
- `analytics` - Analyse- en trackingtools

## Inhoudssegmentatie

Ons platform ondersteunt logische inhoudssegmentatie binnen MDX-bestanden. Dit maakt inhoud beter onderhoudbaar en biedt een betere structuur voor gidsen, terwijl ze leesbaar blijven in standaard markdown-editors.

### Segmentatieformaat

Om je inhoud te segmenteren, gebruik je de volgende syntax:

```md
---section:sectienaam
Je markdown-inhoud komt hier.
Inhoud kan meerdere alinea's beslaan.
---
```

### Standaardsecties

We raden aan deze standaard sectienamen te gebruiken voor gidsen:

- `intro`: Introductie en overzicht van de migratie
- `before`: Vereisten en voorbereidingsstappen
- `steps`: Het stap-voor-stap migratieproces
- `troubleshooting`: Veelvoorkomende problemen en oplossingen
- `outro`: Conclusie en laatste opmerkingen

### Voorbeeld van Gesegmenteerde Inhoud

Dit is hoe een gesegmenteerde gids gestructureerd moet zijn:

```md
---
title: 'Migreren van Service A naar Service B'
description: 'Stap-voor-stap handleiding voor het overstappen van Service A naar Service B'
difficulty: 'beginner'
timeRequired: '30 minuten'
sourceService: 'Service A'
targetService: 'Service B'
date: '2025-04-08'
author: 'Switch-to.EU Team'
---

---section:intro
# Migreren van Service A naar Service B

Service B is een veilig EU-gebaseerd alternatief voor Service A. Deze gids helpt je bij het migreren van je gegevens.

## Waarom Overstappen naar Service B?

De belangrijkste voordelen van Service B zijn:
- EU-gebaseerde infrastructuur
- Verbeterde privacyfuncties
- AVG-naleving
---

---section:before
## Voordat Je Begint

### Vereisten
- Een actief Service A-account
- Een computer met internettoegang
- Ongeveer 30 minuten tijd

### Wat Je Nodig Hebt
- Een veilig wachtwoord voor je nieuwe Service B-account
---

---section:steps
## Stap 1: Maak een Service B-Account

1. Bezoek de website van Service B
2. Klik op "Aanmelden"
3. Voer je gegevens in en maak je account aan

## Stap 2: Exporteer Je Gegevens uit Service A

1. Log in op Service A
2. Ga naar Instellingen
3. Zoek de Exportoptie en download je gegevens
---

---section:troubleshooting
## Probleemoplossing

### Veelvoorkomende Problemen
- **Inlogproblemen**: Zorg ervoor dat je inloggegevens correct zijn
- **Ontbrekende gegevens**: Controleer of alle gegevens correct zijn geëxporteerd

### Hulp Krijgen
Als je problemen ondervindt, neem contact op met het ondersteuningsteam van Service B
---

---section:outro
## Conclusie

Gefeliciteerd! Je bent succesvol gemigreerd van Service A naar Service B.

Vergeet niet om je inloggegevens bij te werken op andere diensten die mogelijk gekoppeld zijn.
---
```

### Achterwaartse Compatibiliteit

Het segmentatiesysteem is achterwaarts compatibel. Niet-gesegmenteerde inhoud blijft correct werken. Als je bestaande gidsen bijwerkt, overweeg dan om segmentatie toe te voegen om de onderhoudbaarheid te verbeteren.

## Een Nieuwe Gids Maken

Om een nieuwe migratiegids te maken:

1. Bepaal de juiste categorie voor je gids
2. Maak een nieuwe map met een beschrijvende naam (bijv. `gmail-naar-protonmail`)
3. Kopieer de sjabloon van `/content/templates/guide-template.mdx`
4. Vul alle secties van de sjabloon in
5. Voeg screenshots toe aan de afbeeldingenmap

## Frontmatter Structuur

Elke gids moet frontmatter aan het begin van het MDX-bestand bevatten met de volgende velden:

```mdx
---
title: "Migreren van [Service A] naar [Service B]"
description: "Een stapsgewijze handleiding om je te helpen migreren van [Service A] naar [Service B], een EU-gebaseerd alternatief."
publishedAt: "JJJJ-MM-DD"
updatedAt: "JJJJ-MM-DD"
author: "Jouw Naam"
difficulty: "beginner|intermediate|advanced"
timeRequired: "X minuten|uren"
sourceService: "Service A"
targetService: "Service B"
sourceServiceUrl: "https://example.com"
targetServiceUrl: "https://eu-example.eu"
---
```

## Schrijfrichtlijnen

Om consistentie in alle gidsen te waarborgen:

1. **Wees Duidelijk en Beknopt** - Gebruik eenvoudige taal en korte zinnen
2. **Stap-voor-Stap Formaat** - Nummer elke stap duidelijk en voeg screenshots toe
3. **Benadruk Verschillen** - Vermeld belangrijke verschillen tussen de bron- en doelservices
4. **Voeg Probleemoplossing Toe** - Voeg een sectie toe voor veelvoorkomende problemen en oplossingen
5. **Houd Het Actueel** - Update gidsen wanneer services veranderen

## Je Gids Testen

Voordat je een gids indient:

1. Volg je eigen instructies van begin tot eind
2. Test op verschillende apparaten en browsers indien relevant
3. Laat iemand anders de gids beoordelen en testen

Bedankt voor je bijdrage aan Switch-to.EU en het helpen van gebruikers bij het migreren naar EU-diensten!