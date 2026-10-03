# How to Build the Custom GPT

## Recommended GPT Name
Marketplace Property Ad Engine

## Description
Creates one Ideal-Buyer-Persona-specific Facebook Marketplace real estate ad from a URL, address, transcript, brochure, or pasted property information. It identifies the strongest reason to care, turns features into benefits, scores the draft, revises weak sections, and returns the final ad with photo recommendations and headline alternatives.

## Conversation Starters
- Create a Marketplace ad from this property URL.
- Use this property plus my Ideal Buyer Persona to write the ad.
- Focus this ad on the oversized lot.
- Create a second ad around a different main reason and make it at least 75% different.
- Review this Marketplace ad against the 5 Rules and improve it.

## Build Steps
1. Open the GPT builder in ChatGPT.
2. Create a new GPT.
3. Use the recommended name and description.
4. Paste `prompts/GPT_INSTRUCTIONS.md` into Instructions.
5. Upload these Knowledge files:
   - `prompts/BUYER_INTELLIGENCE_REFERENCE.md`
   - `config/decision_engine.json`
   - `config/marketplace_rubric.json`
6. Enable web search if you want the GPT to research public property/community URLs.
7. Test with several properties before sharing.
8. Confirm it does not invent facts and follows fair housing requirements.

## Recommended User Input
The user can simply provide a property URL or property information. Better results are possible when they also provide:
- Ideal Buyer Persona
- Optional main angle
- Phone
- Email
- Lead-capture website (optional but recommended)

## Output
The GPT returns:
1. Headline
2. Marketplace Ad
3. Recommended Photo Order
4. Three Headline Variants
