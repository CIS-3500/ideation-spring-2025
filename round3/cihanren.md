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
As a student, I want to summarize an abstract so that I can understand the paper quickly before reading it in full.

As a researcher, I want to extract citations in APA format so that I can add them directly to my bibliography.

As a grad student, I want to see a list of related papers so that I can explore other research on the same topic.

As a TA, I want to explain complex method sections using ChatGPT so that I can better help my students during office hours.

As a writer, I want to generate a BibTeX entry for a paper so that I can easily import it into my LaTeX documents.

As a student writing a literature review, I want to extract key findings from multiple papers so that I can compare results across studies quickly.

As a PhD candidate, I want to save my favorite papers in a reading list within the extension so that I can revisit them later without searching again.

As a professor, I want to auto-generate discussion questions from a paper’s abstract and conclusion so that I can use them in class.

As a non-native English speaker, I want to rephrase complex academic language in simpler terms so that I can understand the paper more easily.

As a grant writer, I want to extract relevant citations and summarize related research so that I can support my proposal with existing work.

As a STEM major, I want to explain technical jargon in the method section so that I can grasp the procedure used in the study.

As a research assistant, I want to export structured data (title, abstract, author, publication date) to a CSV file so that I can manage my research library.

As a science communicator, I want to turn academic papers into layperson summaries so that I can share insights with a broader audience.

As a student applying to grad school, I want to generate a concise summary of a professor’s recent publications so that I can reference their work in my statement.

As a course designer, I want to extract and analyze recurring keywords in selected research papers so that I can identify trending topics for curriculum updates.



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
