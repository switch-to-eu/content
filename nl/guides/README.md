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