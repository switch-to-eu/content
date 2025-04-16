# Guide Contributor's Documentation

Welcome to the Switch-to.EU guides documentation! This README provides everything you need to know about creating and maintaining migration guides for EU service alternatives.

## Guide Structure

Each migration guide should be placed in its appropriate category directory and follow this structure:

```
/content/guides/[category]/[service-name]/
├── index.mdx          # The main guide content
└── images/            # Images folder for screenshots and diagrams
    ├── step1.png
    ├── step2.png
    └── ...
```

## Guide Categories

Guides are organized by service category:

- `email` - Email services
- `storage` - Cloud storage services
- `messaging` - Chat and messaging applications
- `productivity` - Office and productivity tools
- `analytics` - Analytics and tracking tools

## Creating a New Guide

To create a new migration guide:

1. Identify the appropriate category for your guide
2. Create a new folder with a descriptive name (e.g., `gmail-to-protonmail`)
3. Copy the template from `/content/templates/guide-template.mdx`
4. Fill in all sections of the template
5. Add screenshots to the images folder

## Frontmatter Structure

Each guide should include frontmatter at the top of the MDX file with the following fields:

```mdx
---
title: "Migrating from [Service A] to [Service B]"
description: "A step-by-step guide to help you migrate from [Service A] to [Service B], an EU-based alternative."
publishedAt: "YYYY-MM-DD"
updatedAt: "YYYY-MM-DD"
author: "Your Name"
difficulty: "beginner|intermediate|advanced"
timeRequired: "X minutes|hours"
sourceService: "Service A"
targetService: "Service B"
sourceServiceUrl: "https://example.com"
targetServiceUrl: "https://eu-example.eu"
---
```

## Writing Guidelines

To ensure consistency across all guides:

1. **Be Clear and Concise** - Use simple language and short sentences
2. **Step-by-Step Format** - Number each step clearly and include screenshots
3. **Highlight Differences** - Note key differences between the source and target services
4. **Include Troubleshooting** - Add a section for common issues and solutions
5. **Keep It Current** - Update guides when services change

## Testing Your Guide

Before submitting a guide:

1. Follow your own instructions from start to finish
2. Test on different devices and browsers if relevant
3. Have someone else review and test the guide

Thank you for contributing to Switch-to.EU and helping users migrate to EU services!