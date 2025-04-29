# Chrome Extension Idea: BuyAdvisor — Amazon Product Reviewer & GPT Prompt Builder

## Authors  
- Claire Zhao (clairezz)
- Ioannis Kalaitzidis (jokala)
- Maria Ramos ()
- Chaelsey Park (chaelsey)

---

## Problem Statement  
When evaluating a product on Amazon, buyers often face decision fatigue. Reviews are abundant but noisy, critical specs are scattered, and it’s hard to judge **whether a product is actually a good fit for their use case**. This issue is especially frustrating for students or budget-conscious consumers who want fast, reliable purchasing decisions with minimal effort.

Large Language Models (LLMs) like ChatGPT are often used to summarize reviews or compare products — but users must manually copy and paste information, often across multiple tabs, and craft a good prompt themselves. This is time-consuming and inefficient.

**BuyAdvisor solves this** by automatically extracting product information, specs, and top reviews from the Amazon product page the user is currently viewing and assembling **ready-to-use GPT prompts** that help them quickly decide whether to buy, wait, or consider alternatives.

---

## Target Audience  
- College students buying electronics, dorm supplies, books, etc.  
- First-time buyers evaluating expensive or technical products.  
- Budget shoppers trying to make smart choices without reading 100+ reviews.  
- Users already accustomed to pasting info into ChatGPT for product research.

---

## Description  
BuyAdvisor is a Chrome extension that activates when the user visits an Amazon product page. It:
- Extracts the **product title, price, star rating**, and **ASIN**
- Parses the first 20–50 most helpful **review cards**
- Analyzes review sentiment (positive/negative themes) using basic keyword clustering
- Optionally stores multiple products for comparison
- Generates one or more **LLM-ready prompts** for evaluating whether the product is worth buying based on summarized data

The user can then copy and paste the prompt into a tool like ChatGPT for quick, intelligent decision-making.

---

## Selling Points  
1. **No Copy-Pasting Needed** — All relevant content (price, reviews, specs) extracted and structured instantly.
2. **LLM-Optimized Prompt Generation** — Structured prompts tailored for product recommendation, comparison, or concern-spotting.
3. **Multi-Product Comparison** — Save multiple products and generate a comparative GPT prompt in one click.
4. **Fast Sentiment Extraction** — Lightweight keyword-based clustering gives a “what people liked vs. hated” view without any external APIs.
5. **Privacy-Respecting** — All processing is local. No scraping of Amazon’s servers or external API calls needed.

---

## User Stories  
1. As a college student, I want to evaluate if a pair of headphones is worth $130 without reading 500 reviews, so that I can make a confident purchase quickly.  
2. As a price-conscious buyer, I want to compare 3 similar products I’m viewing in different tabs, so I can pick the best-value one.  
3. As a GPT user, I want a prebuilt prompt that summarizes reviews and specs, so I don’t waste time assembling information by hand.  
4. As a user of Chrome extensions, I want to extract review summaries with one click, so I can avoid browser tab overload.  
5. As a shopper, I want to know if a recent product version (v3.0) has specific new problems reviewers are mentioning, so I can avoid defective updates.
6. As a student shopping for tech gear, I want to know what people say about durability so that I don’t waste money on a fragile item.
7. As a user comparing multiple products, I want to generate a side-by-side GPT prompt that includes prices, pros, and cons so that I can make a quick decision.
8. As a shopper on a budget, I want to know if the current price is fair based on reviews and product quality so that I don’t overpay.
9. As someone with specific use cases (e.g., traveling, gaming, studying), I want to prompt GPT to match features with my needs so that I pick the most suitable product.
10. As a buyer overwhelmed by technical specs, I want a summary of key functional differences extracted from reviews so that I can understand them quickly.
11. As a frequent Amazon user, I want to save product summaries locally so that I can review them all before checkout.
12. As a casual user of GPT, I want pre-written prompts that are clean and informative so that I don’t have to figure out what to ask.
13. As a parent buying electronics for a child, I want GPT to highlight potential risks or frustrations based on other parents’ reviews so that I make a safer purchase.
14. As a user looking at a brand-new product with few reviews, I want GPT to tell me what risks I’m taking so that I can decide whether to wait.
15. As a shopper evaluating version upgrades (e.g., v3.0 vs. v2.0), I want GPT to identify what changed and whether it improved so that I make an informed upgrade decision.
16. As a visually-impaired shopper using screen readers, I want GPT-generated summaries to be short and clearly structured so that I can understand them with assistive tech.
17. As a researcher studying user sentiment, I want to export review summaries to a CSV file so that I can analyze trends offline.
18. As a Chrome user, I want the extension to trigger automatically on supported Amazon pages so that I don't have to click anything to extract data.
19. As a shopper looking for long-term value, I want GPT to highlight red flags in durability or warranty complaints so that I avoid regret.
20. As a user doing a bulk purchase (e.g., dorm supplies), I want GPT to rank top 3 value buys from my saved list so that I can buy efficiently.

---

## Example Prompts Generated

**Prompt A – “Should I Buy This?”**
```text
I’m considering buying this product:
- Title: Sony WH-1000XM4
- Price: $129.99
- Rating: 4.6 stars (12,245 reviews)
- Good: battery life, noise cancelling, travel case
- Bad: headband cracking, muffled bass at high volume

Should I buy this now, or are there better alternatives for a student under $150? Keep it under 150 words.
```
**Prompt B – “Compare These 3 Products”**
```text
Compare the following headphones for value, quality, and suitability for college study:
1. Sony WH-1000XM4 — $129.99, 4.6★, strong ANC, fragile build
2. Bose QC45 — $179.99, 4.7★, best for comfort, high price
3. JBL Tune 750 — $89.00, 4.3★, solid mids, no ANC

Rank them by recommendation strength and give a 1-sentence summary for each.
```

## Technical Implementation

### A. Architecture Overview

| Component | Role |
|-----------|------|
| **Content Script** | Extracts product metadata, specs, and reviews from the loaded DOM. |
| **Popup Script** | Displays extracted data and allows the user to copy GPT prompts easily. |
| **Background Script** | Stores product information across tabs (for multi-product comparison). |
| **Storage** | Uses `chrome.storage.local` to persist saved product summaries locally. |

---

### B. Key DOM Selectors

| Data | Selector |
|------|----------|
| **Title** | `#productTitle` |
| **Price** | `#priceblock_ourprice` or `#priceblock_dealprice` |
| **Specs** | `#feature-bullets` |
| **ASIN** | Extracted from product information section or parsed from URL (`/dp/ASIN`) |
| **Reviews** | `document.querySelectorAll('[data-hook="review"]')` — extract top review cards |

---

### C. Review Sentiment Extraction (Lightweight, No ML)

- Parse the first 20–50 review titles and bodies.
- Count the presence of **positive** keywords (e.g., “great”, “love”, “works well”) versus **negative** keywords (e.g., “broke”, “terrible”, “waste”).
- Cluster and count frequently mentioned nouns and phrases (e.g., “battery life”, “headphones”, “comfort fit”) to identify top positive and negative themes.

---

## Notes

### Limitations
- Only works on `amazon.com` (no support for international Amazon domains in the MVP).
- No direct integration with ChatGPT — the user manually copies and pastes prompts.
- Only analyzes a limited number of reviews per product to remain within GPT context window (e.g., 4,096 tokens).

### Future Enhancements
- Add a Chrome right-click shortcut: “Generate GPT prompt for this product.”
- Offer tone customization options for generated prompts (e.g., “convince me to buy,” “roast this product,” “recommend for parents”).
- Add optional GPT API integration (users input their API key to automate prompt sending).

---

## References & Inspiration

- Amazon’s DOM structure and element naming conventions (reverse-engineered through DevTools).
- GPT-4 and GPT-3.5 best practices for prompt engineering and summarization tasks.
- CamelCamelCamel.com for potential future price history integration (scraping optional).
- Prior CIS-3500 project inspiration: [Penn Course GPT Assistant].
