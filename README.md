# Facebook Marketplace Real Estate Writing Engine

A buyer-first system for creating one Facebook Marketplace real estate ad from a URL, address, transcript, brochure, MLS description, community information, or pasted property details.

The engine follows the same framework taught in the New Construction Facebook Marketplace Real Estate Ads Best Practices guide:

1. Know the Ideal Buyer Persona
2. Give them one main reason to care
3. Turn features into benefits
4. Make the ad easy to read and believe
5. Make the next step simple

Primary goal: generate qualified messages and leads. Clicks and saves are useful signals, but they are not the final goal.

## What This System Produces

Each run returns:

1. One primary headline
2. One complete Facebook Marketplace ad
3. A recommended photo order
4. Three alternative headlines

The engine performs buyer analysis, strategy selection, scoring, and rewriting internally.

## Accepted Inputs

Provide any one of these:

- Property URL
- Community or builder URL
- Complete address
- MLS or listing description
- Brochure or flyer
- Transcript
- Pasted property details

Recommended when available:

- Ideal Buyer Persona
- Optional angle or feature emphasis
- Agent phone number
- Agent email
- Lead-capture website

If an Ideal Buyer Persona is supplied, use it as the primary buyer reference. If one is not supplied, infer one from supported property, price, location, and use information without using protected traits.

## Core Workflow

### 1. Property Intelligence
Extract only supported facts. Never invent pricing, incentives, availability, views, amenities, financing, schools, commute times, zoning, legal use, scarcity, or future potential.

### 2. Ideal Buyer Persona
Determine who is most likely to care about the property and why. Focus on housing needs, motivations, lifestyle and use needs, buying behavior, concerns, timing, and financial readiness when appropriate.

### 3. One Main Reason to Care
Choose the strongest supported reason the Ideal Buyer Persona should care. The headline, opening, benefits, and supporting details should reinforce that same story.

If several strong reasons exist, they can become separate ads. Each alternate ad should focus on a different main reason and be at least 75% different from the others.

### 4. Feature to Benefit
Translate important property facts into buyer outcomes. Ask why the Ideal Buyer Persona cares and how the feature could make life better, easier, more convenient, more enjoyable, or solve a problem.

### 5. Offer
Package the property around something the Ideal Buyer Persona already wants, needs, or is trying to solve. An offer can be lifestyle, convenience, freedom, simplicity, opportunity, or a verified financial incentive.

### 6. Headline and Opening
The headline earns attention. The first 1-2 lines continue the same reason that made the buyer stop.

### 7. Specific Proof
Prefer supported specifics over empty adjectives. Claims such as great location, huge, luxury, or low-maintenance should be supported with facts when possible.

### 8. Buyer Life
Help the buyer picture what the feature or benefit could mean in everyday life.

### 9. Easy-to-Scan Copy
Use short paragraphs, clear sections, and bullets when helpful. Long copy is acceptable when the decision requires explanation, but the main reason to care should be easy to find.

### 10. Simple Next Step
Use one clear primary CTA, normally an on-platform Marketplace message with a memorable keyword and a clear promise of what the buyer will receive.

Also include phone and email when supplied. A website at the end of the CTA is optional but recommended. When a website is supplied, add a short blurb explaining what the buyer can get there, then include the website URL. Prefer a simple lead-capture page that collects name, email, and phone and sends the lead into the agent's CRM. An IDX page can work, but a dedicated lead-capture page is preferred.

## Marketplace Category Note

When Facebook's current categories allow it, test the Miscellaneous category instead of automatically using the standard Homes for Sale category when doing so provides better control over a descriptive custom headline. This is a headline-control test, not a claim that Facebook gives Miscellaneous posts more reach.

## Internal Scoring

The engine scores the draft for:

- Headline clarity
- Reason-to-stop strength
- Ideal Buyer Persona alignment
- One-main-idea focus
- Problem/desire alignment
- Offer strength
- Feature-to-benefit conversion
- Specific proof
- Buyer-life visualization
- Readability and scanability
- CTA strength
- Qualified-lead likelihood
- Duplicate-risk control
- Compliance and factual support

Every category must score at least 8.5 and the weighted score must reach at least 8.8. The engine revises weak sections up to five times.

## Repository Structure

```text
marketplace-writing-engine/
├── README.md
├── GPT_SETUP.md
├── prompts/
│   ├── GPT_INSTRUCTIONS.md
│   ├── STANDALONE_PROMPT.md
│   └── BUYER_INTELLIGENCE_REFERENCE.md
├── config/
│   ├── decision_engine.json
│   └── marketplace_rubric.json
└── skills/
    └── marketplace-writing-engine/
        └── SKILL.md
```

## Two Ways to Use It

### Custom GPT
Paste `prompts/GPT_INSTRUCTIONS.md` into the GPT Instructions field. Upload `prompts/BUYER_INTELLIGENCE_REFERENCE.md`, `config/decision_engine.json`, and `config/marketplace_rubric.json` as Knowledge.

### Standalone Prompt
Paste `prompts/STANDALONE_PROMPT.md` into ChatGPT, Claude, or another capable AI tool, then provide the property information and Ideal Buyer Persona when available.

## Recommended Tracking

Track:

- Property
- Ideal Buyer Persona
- Main reason to care
- Offer/angle
- Headline
- Views/clicks
- Saves
- Messages
- Qualified conversations
- Appointments/showings
- Closed transactions

Use results to improve future ads without treating one winner as permanent proof.
