# Chrome Extension Idea: Discord Ticket Extractor

## Authors

Cecilia Zhang, Garrett Kirsch

## Problem Statement

Many Discord servers use ticketing systems to handle support requests, reports, or feedback. These tickets often generate long transcripts that are hard to parse or extract useful insights from. Whether viewing the ticket channel directly or reviewing transcripts after closure, users often have to scroll through cluttered messages to identify key details.

Server admins, moderators, and community managers need a better way to generate concise summaries of ticket conversations for reporting, documentation, or follow-up actions. This extension solves that gap by allowing users to extract and immediately summarize ticket content using LLMs like ChatGPT.

## Target Audience

- Content creators summarizing chat highlights for videos or blogs.
- Community managers archiving tickets to maintain a record of behavior, content, and issues.
- Discord users who use LLMs to summarize, analyze, or reformat long threads.

## Description

This Chrome extension extracts and formats Discord ticket transcripts from web-based servers. It strips out bot responses, repetitive system messages, and UI clutter—leaving just the clean conversation between the user and staff. The output is ready to copy into an LLM for summarization or to archive for records.

## Selling Points

1. One-click extraction from any ticket channel on the web.
2. Clean formatting optimized for LLM input or archiving.
3. Filters out non-essential system/bot messages.
4. Export as plain text or markdown for internal docs or reports.
5. Lightweight and privacy-safe (runs fully in-browser).

## User Stories

1. As a support moderator, I want to extract a ticket conversation so that I can summarize it with ChatGPT.
2. As a server admin, I want to archive and organize ticket transcripts so that I can reference them later in case of disputes.
3. As a new support mod, I want to learn from previous tickets so that I can train myself on standard responses.
4. As a project manager, I want to extract tickets related to a specific topic so that I can track issue trends.
5. As a mod lead, I want to create summaries of user issues so that I can present them in team meetings.
6. As a moderator, I want to save a ticket conversation before deleting the channel so that I retain a record of the discussion.
7. As a Discord admin, I want to document moderation actions in tickets so that I can build a case log.
8. As a community manager, I want to extract entire support conversations so that I can create FAQ entries or documentation.
9. As a community manager, I want to generate a quick summary of a ticket so that I can report common issues to the team without reading the full transcript.
10. As a support lead, I want to review summarized versions of tickets from the past week so that I can identify patterns and improve our response templates.

## Notes
Focus on compatibility with popular bots (i.e. Ticket Tool).

Could optionally add a "highlight important messages" feature using keyword detection.

## References & Inspiration

https://tickettool.xyz/