# Chrome Extension Idea: ReviewDigest

## Authors

Winnie Wang, Kevin Yang-Li, Wesley Liu

## Problem Statement

When users shop online, especially on platforms like Amazon, they are often overwhelmed by the sheer volume of product reviews. Sorting through hundreds of opinions to identify genuine pros and cons takes time and effort, and many buyers abandon the process or make poorly informed decisions. Additionally, users who want to use LLMs like ChatGPT, Gemini, or Claude to help them summarize reviews must manually copy and format the reviews, open a separate tab, and craft prompts from scratch. This Chrome extension addresses these pain points by automating review extraction and LLM interaction in a seamless, customizable workflow.

## Target Audience

The primary audience includes online shoppers who research reviews before purchasing products. This includes tech enthusiasts, parents, students, professionals—anyone who values informed decisions but wants to save time. Users are likely familiar with Chrome extensions and large language models but want a quicker, smarter way to use them in the context of e-commerce.

## Description

This is a Chrome Extension that scrapes all visible reviews from a selected Amazon product page, formats them, and then opens a new tab with the user’s chosen LLM (e.g., ChatGPT, Gemini, DeepSeek). It pastes the reviews along with a personalized, pre-saved prompt into the LLM interface. The prompt can ask the model to summarize the main pros and cons, highlight recurring complaints or praises, or compare with alternative products. Users can customize and save their default prompt in the extension’s settings for future use.

## Selling Points

1. One-click extraction and summarization of Amazon reviews using any LLM.
2. Works with ChatGPT, DeepSeek, Gemini, Claude, and other popular chatbots.
3. Personalized prompts let users tailor summaries for what they care about (e.g., durability, ease of use, etc.).
4. Auto-formatting of reviews into clean, LLM-friendly input (e.g., bullet points, separated by sentiment).
5. Saves time by eliminating repetitive manual tasks like copying and pasting.
6. Ideal for comparing multiple products quickly or making last-minute buying decisions with clarity.

## User Stories

As an online shopper, I want to quickly see the main pros and cons of a product without reading hundreds of reviews.
As a tech-savvy buyer, I want to send reviews to ChatGPT with a click and get a summarized response tailored to my needs.
As a frequent Amazon user, I want to reuse a prompt that focuses on build quality and customer servicein every product I evaluate.
As a decision-maker, I want to compare two similar products by getting LLM-generated summaries of each.
As a user, I want the extension to remember my preferred LLM and default prompt so that the process is seamless every time.
As a researcher, I want to extract structured review summaries to track sentiment across multiple products.
As a Chrome user, I want the interface to be lightweight and work reliably across Amazon’s product page layouts.
As a user, I want to eventually export summaries or share them with friends to help others make informed choices.
As a student shopping on a budget, I want to highlight common issues with cheaper products to avoid bad purchases.
As a parent buying toys, I want to know if certain safety concerns are raised frequently in reviews.
As a visually impaired user, I want the extension to support screen readers and keyboard navigation.
As a privacy-conscious shopper, I want to know what data the extension accesses and be able to disable features I don’t use.
As a reviewer myself, I want to quickly scan what other people are saying before deciding whether my experience is unique.
As a casual user, I want to understand which LLM is best for summarization so I can make the right choice in settings.
As someone shopping on mobile via desktop mode, I want the extension to adapt to different screen layouts or mobile web views.

## Notes

While this would be a first Chrome extension project, it seems very feasible. The main challenges would likely be:
Handling review pagination on Amazon.
Creating smooth cross-tab LLM injection (likely simulating keyboard input or clipboard pasting).
Dealing with rate limits or UI changes in third-party LLMs.
Making sure formatting stays clean and readable for LLMs to interpret correctly.

## References & Inspiration

ChatGPT Chrome Extensions for UX inspiration
Prompt engineering guides from OpenAI and DeepSeek
