---
name: service-research
description: Research methodology for evaluating tech services for switch-to.eu. Covers privacy analysis, feature comparison, community sentiment gathering, and EU-specific considerations.
---

# Service Research for switch-to.eu

Methodology and checklists for researching tech services through a privacy-first, European-alternative lens.

## Privacy & Data Evaluation Checklist

### Data sovereignty
- [ ] Where are servers physically located? (Country, ideally city)
- [ ] Which legal jurisdiction governs the data?
- [ ] Is the company EU-based or subject to EU law?
- [ ] Are they subject to US CLOUD Act, FISA, or similar?
- [ ] Do they use US-based infrastructure providers (AWS, Google Cloud, Azure)?

### Encryption
- [ ] Is data encrypted in transit? (TLS version)
- [ ] Is data encrypted at rest? (Algorithm)
- [ ] Who holds the encryption keys? (Company or user)
- [ ] Is there end-to-end encryption? For which features?
- [ ] Is there zero-knowledge architecture?

### Data practices
- [ ] What data do they collect beyond what's needed for the service?
- [ ] Do they use analytics trackers? Which ones?
- [ ] Do they share data with third parties? For what purpose?
- [ ] Can you export all your data? In what format?
- [ ] Can you delete your account? How long until data is purged?
- [ ] Is there a published Data Processing Agreement?

### Track record
- [ ] Any known data breaches?
- [ ] Any controversies about privacy?
- [ ] Have they had independent security audits? Published results?
- [ ] What is their response time to security disclosures?

## Open Source Evaluation

- [ ] What license? (MIT, GPL, AGPL, Apache, proprietary, open-core)
- [ ] Is the client open source? The server?
- [ ] Is there a public git repository? How active is it?
- [ ] Are builds reproducible?
- [ ] Is there meaningful community contribution or is it "source available" with no external PRs?

## Feature Evaluation Framework

When comparing a service to its mainstream alternative, evaluate:

1. **Core functionality**: Does it do the main job adequately?
2. **Migration path**: How hard is it to switch? Import tools available?
3. **Ecosystem integration**: Does it work with other tools people use?
4. **Collaboration**: Can you work with people who use the mainstream alternative?
5. **Mobile support**: Quality of mobile apps
6. **Offline capability**: Works without internet?
7. **API/extensibility**: Can power users extend it?

## Community Sentiment Research

### Where to look
- Reddit: r/privacy, r/selfhosted, r/degoogle, r/europrivacy, service-specific subreddits
- Hacker News discussions
- Mastodon/Fediverse privacy communities
- Product Hunt reviews
- Trustpilot and similar review platforms

### What to track
- Recurring praise themes (what do people consistently like?)
- Recurring complaint themes (what frustrates people?)
- Migration stories (what did they switch from? How was the transition?)
- Deal-breakers mentioned (what made people leave?)
- Comparison opinions (how does it compare to alternatives in practice?)

### How to report
- Aggregate themes, don't cherry-pick individual opinions
- Note frequency: "Several users mentioned..." vs "One user reported..."
- Distinguish between old complaints (possibly fixed) and recent ones
- Include both positive and negative sentiment fairly

## EU & European Context

- Is the company headquartered in the EU/EEA/Switzerland?
- Do they explicitly comply with GDPR?
- Is there a local EU entity or just a US company with EU users?
- Do they accept SEPA, iDEAL, Bancontact, or other EU payment methods?
- Is the interface available in European languages beyond English?
- Are there specific EU pricing tiers or is it USD-only?

## Reddit Research Strategy

Search for:
- `[service name] reddit review` — general sentiment
- `[service name] reddit problems` — known issues
- `[service name] reddit privacy` — privacy concerns
- `[service name] reddit vs [mainstream]` — comparisons
- `[service name] reddit migration` or `switched to [service]` — migration stories
- `r/privacy [service name]` — the r/privacy community's take
- `r/selfhosted [service name]` — for self-hostable services
- `r/degoogle [service name]` or `r/deamazon` — alternative-seeking communities

When summarizing Reddit sentiment:
- Note how many people echo the same point (one person vs recurring theme)
- Distinguish between power users and casual users
- Note the date — old complaints may be fixed
- Look for patterns, not individual opinions

**Reddit 403 fallback**: Reddit blocks direct page fetches. Strategy:
1. Use WebSearch with site:reddit.com queries (snippets contain opinions)
2. Try old.reddit.com URLs with WebFetch
3. If fully blocked, work from search snippets and note the limitation

## Source Quality Ranking

When sources conflict, prioritize:
1. Official documentation (privacy policy, ToS, published specs)
2. Independent security audits (published by known firms)
3. Reputable tech journalism (Ars Technica, The Verge, TechCrunch, Wired)
4. Privacy-focused reviewers (PrivacyGuides, RestorePrivacy, ThatOnePrivacySite)
5. Community consensus on Reddit (multiple users, recent, consistent)
6. Individual user reports (edge cases only)
7. Company blog posts (marketing unless independently verified)

## Recommendation Criteria

**Recommend** when the service:
- Provides a meaningful alternative to mainstream (usually US Big Tech)
- Has clear, honest privacy practices
- Ideally EU-based, or at minimum GDPR-compliant with EU data storage
- Has a sustainable business model
- Is usable enough for non-technical users

**Recommend with caveats** when:
- Technically excellent but has privacy trade-offs
- Privacy-excellent but has usability issues
- Recently changed ownership or business model
- Had breaches but handled them responsibly

**Do not recommend** when:
- Deceptive privacy practices
- Subject to mandatory backdoor jurisdictions with no technical mitigation
- History of poorly handled breaches
- Shut down or acquired by a company with poor privacy track record

## Pricing Research

- Always check pricing in EUR
- Note if pricing is per-user, per-device, or per-storage
- Compare free tier limitations honestly
- Note if pricing has changed recently (and in which direction)
- Check for student/nonprofit discounts
- Note payment methods (especially privacy-friendly options like cash/crypto)
