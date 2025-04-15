# Chrome Extension Idea: [Title]

## Authors

Michael Ren

## Problem Statement

Students and researchers often spend considerable time copying and pasting information from academic research pages into ChatGPT or citation tools to better understand the content or generate citations. Extracting relevant information like abstracts, methods, and references can be tedious, and switching between tabs breaks workflow. Existing solutions either require multiple steps or don’t integrate with LLMs efficiently. Our extension solves this by automatically extracting structured data from research platforms like Google Scholar or arXiv and offering one-click LLM-powered prompts for summarizing, explaining, and citing content — all from within the same browser tab.


## Target Audience

The primary users of this extension are university students, graduate researchers, academic writers, and professionals in research-intensive roles. These users frequently read academic papers, write literature reviews, or cite scholarly work. They are tech-savvy, time-constrained, and familiar with tools like ChatGPT and Google Scholar, making them ideal users for an integrated productivity assistant like this.


## Description

The Smart Academic Assistant is a Chrome extension that extracts metadata from research paper pages and allows users to interact with the content using AI-powered tools. Users can summarize abstracts, explain methods, generate formatted citations, and get related paper suggestions — all within a clean popup on the same page.

## Selling Points

1. One-click summarization of complex abstracts using GPT.

2. Instant generation of citations in APA or BibTeX format.

3. Structured data extraction from well-formatted sources like Google Scholar and arXiv.

4. Built-in AI prompts tailored for academic workflows (e.g., "Explain this method section").

5. Saves time and reduces cognitive load by eliminating copy-paste between tabs.

## User Stories

_[List user stories that describe the main features of your Chrome Extension. Use the following template: "As a [user role], I want to [goal] so that [benefit]." Fill in the brackets with the appropriate information. For Round 1, write 5 user stories; Round 2, write 10 user stories; Round 3, write 15 user stories.]_

## Notes

We plan to start with Google Scholar and arXiv due to their structured HTML or available APIs.

Integration with LLMs like ChatGPT requires using the OpenAI API, which might need a user-provided API key.

We’ll use DOM parsing to extract fields like title, authors, abstract, and references.

Future versions could support PDF extraction or user-saved “paper collections.”

UX is a priority — the popup must be simple and fast.
## References & Inspiration

arXiv API

Google Scholar structure guide

Semantic Scholar

ZoteroBib

OpenAI ChatGPT summarization use-cases

Chrome extension architecture docs: Chrome Extensions Docs
