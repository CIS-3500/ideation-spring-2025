# Chrome Extension Idea: Prospector

## Authors

Kevin Yang-Li

## Problem Statement

Users often spend a lot of time looking for relevant reviews when shopping on platforms like Amazon or eBay. Many reviews are lengthy, repetitive, or include irrelevant details. Shoppers who are trying to make quick, informed purchasing decisions want concise, trustworthy summaries of the main pros and cons of a product — without wading through dozens of reviews. This is where the Chrome extension comes in.

## Target Audience

The target audience includes online shoppers who:
- Frequently purchase products on Amazon, eBay, or similar platforms
- Are comparison shoppers or deal-hunters who want to evaluate products efficiently
- Value quick decision-making aided by trustworthy summaries
- Are overwhelmed by long or unstructured reviews
- May not have the technical skill to do manual filtering or review analysis

This includes tech-savvy consumers, students, professionals, and budget-conscious shoppers.

## Description

**Prospector** is a Chrome extension that scrapes user reviews from Amazon and eBay product pages and allows the user to easily paste the information in a well-formatted manner in an LLM (such as chatGPT or other ones that the user can choose).

## Selling Points

1. AI-generated summaries tailored to each product page
2. Keyword targeting: Users can filter pros/cons by what's important to them
3. Clean, non-intrusive UI that appears as a floating widget or sidebar
4. Saves time and reduces buyer’s remorse by highlighting patterns in reviews

## User Stories

1. As a shopper, I want to see a list of top pros and cons so that I don't have to read every review.
2. As a user, I want to input what I care about (e.g., "battery life") so that the summaries reflect my needs.
3. As a comparison shopper, I want to use the extension on multiple product pages to quickly compare them.
4. As a casual user, I want the extension to run automatically without needing setup so that I can get instant insights.
5. As a visually impaired user, I want accessible output so that I can hear the summaries via screen reader.

## Notes

- Scraping Amazon and eBay content might require dynamic content handling (e.g., lazy-loaded reviews).
- Privacy and speed are important: consider local summarization for faster feedback (or an offline model in the future).
- MVP should focus only on Amazon reviews before expanding to other platforms.
- Potential future features: sentiment scoring, reviewer credibility ranking, review timeline (how feedback changes over time).

## References & Inspiration

- [Fakespot](https://www.fakespot.com/) – Fake review detection and summary tool
- [ReviewMeta](https://reviewmeta.com/) – Amazon review analyzer