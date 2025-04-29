# Chrome Extension Idea: BuyAdvisor — Amazon Product Reviewer & GPT Prompt Builder

## Authors  
Ioannis Kalaitzidis (jokala)  
[Additional team member names + PennKeys]

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
