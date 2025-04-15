# Chrome Extension Idea: Breaking Chains

## Authors

Emma Twitmyer, Allen Liu, Lisa Ayisi-Ahwireng, Luna Chen

## Problem Statement

When email chains become too long, it becomes increasingly difficult to extract relevant information and context. This is due to excessive indentation, multiple participants, and the presence of redundant or unrelated content. The problem worsens when someone new is looped into the conversation mid-thread.

Breaking Chains is a Chrome extension for Gmail that solves this problem by providing users with:
- A concise summary of the entire thread
- A breakdown of each message, with distractions like pleasantries or repeated information filtered out

Users can also engage ChatGPT for suggested replies or to gain clarity about the conversation's content and trajectory.

## Target Audience

This extension is ideal for individuals who frequently manage complex or lengthy email threads, such as:
- Administrators
- Executives
- Project Leads
- Customer Support Teams
- Academic Researchers
- Business Development Professionals

These users often need to understand the full scope of an email conversation without wasting time sifting through noise.

## Description

Breaking Chains integrates seamlessly into Gmail and offers the following functionality:
- A high-level summary of the entire email thread
- A chronological breakdown of individual messages, highlighting unique and relevant content
- Extraction and display of action items or requests
- Integration with ChatGPT for suggested responses or decision-making guidance
- A clean, non-disruptive overlay UI that appears within Gmail for convenient access

## Selling Points

1. Saves Time: Rapidly distills long email threads into key points
2. Reduces Frustration: Strips out fluff, allowing users to focus on what matters
3. Boosts Productivity: Makes it easier to make decisions or reply promptly
4. Improves Accessibility: Presents information in a clearer, more organized format

## User Stories

- As a user, I want the extension to automatically generate a high-level summary of an entire email thread so that I can understand the key points without reading each message.
- As a user, I want the extension to provide a chronological, email-by-email breakdown of the conversation so that I can trace the progression of topics and decisions made.
- As a user, I want the extension to highlight direct requests or action items addressed to me so that I can prioritize my tasks effectively.
- As a user, I want to customize the summarization criteria to prioritize certain keywords or topics so that I can tailor the analysis to my specific needs.
- As a user, I want the extension to categorize emails by purpose (e.g., requests, responses, updates) so that I can quickly identify relevant messages.
- As a user, I want the extension to filter out pleasantries, salutations, and common phrases so that I can focus only on meaningful content.
- As a user, I want the extension to generate suggested responses based on the extracted conversation summary so that I can reply efficiently.
- As a user, I want the extension to allow me to export a summarized thread to a text file or clipboard so that I can share or archive the summary for later use.
- As a user, I want the extension to visually differentiate between different conversation topics using color-coding or labels so that I can easily identify shifts in discussion.
- As a user, I want the extension to notify me of unresolved questions or requests within the conversation so that I can address them promptly.
- As a user, I want to bookmark or pin key messages within the thread so that I can refer back to critical points quickly.
- As a user, I want the extension to support Gmail labels and filters so that I can apply summaries only to specific threads or categories.
- As a user, I want the extension to detect repeated content across replies and collapse them so that I don’t waste time re-reading the same information.
- As a user, I want to view who contributed which key points in the summary so that I can follow up with the right person.
- As a user, I want the option to summarize threads in different tones (formal, concise, detailed) so that the output fits different work contexts.

## Notes

- Technical Challenge: Ensuring robust parsing across email formats, languages, and nested threads
- Privacy Considerations: No data should be stored or transmitted externally without explicit user permission
- Alternative Approaches: Consider expansion to platforms like Outlook or mobile clients
- Future Feature: Allow user-defined rules for filtering or highlighting custom phrases, team names, or tags

## References & Inspiration

Personally inspired by recurring frustrations in navigating long email threads.  
Also encouraged by a shared spreadsheet of brainstormed extension ideas.

Other tools to explore for inspiration:
- [Superhuman](https://superhuman.com/)
- Gmail’s Smart Compose
