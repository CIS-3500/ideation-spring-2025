# Chrome Extension Idea: Caption Capturer

## Authors

Hajoon Park

## Problem Statement

University students often watch recorded lectures via Canvas Panopto, but extracting meaningful content from those lectures to use with Large Language Models (LLMs) is inefficient. Manually taking notes or copying captions wastes time and leads to fragmented study material. Panopto’s built-in transcript is helpful but not optimized for tasks like summarization, Q&A generation, or comprehension checks.

Caption Capturer solves this by automatically extracting lucture video captions and converting them into LLM-ready prompts for summarization, question generation, note-taking, and more.

## Target Audience

College students using Canvas Panopto to watch recorded lectures

Students who use ChatGPT or other LLMs for summarizing, note-taking, or self-quizzing

Non-native English speakers who want help understanding complex lectures

Anyone who prefers AI-powered study methods

## Description

This is a Chrome Extension that works on Canvas-integrated Panopto lecture videos. It extracts transcripts from lecture videos and turns them into LLM-friendly prompts for automatic summarization, quiz creation, translation, and personalized learning.

## Selling Points

1. Lecture-optimized – Tailored specifically for Canvas Panopto lecture formats

2. Transcript to Prompt – Turns raw lecture text into clean prompts instantly

3. Self-quiz feature – Generate multiple choice or short-answer questions from lectures

4. Language support – Translate lectures to your preferred language before prompting

5. Export-ready – Easily copy prompts or export summaries to Notion, markdown, or PDF

## User Stories

As a student, I want to summarize a Panopto lecture so that I can quickly review the content before exams.

As a non-native English speaker, I want to translate the lecture transcript and summarize it in Korean.

As a student using ChatGPT, I want a formatted prompt based on the lecture so that I don’t have to write it from scratch.

As a learner preparing for tests, I want to auto-generate quiz questions from lecture content.

As a busy student, I want to scan a long lecture and get key takeaways in a minute.

## Notes

Captions/transcripts will be accessed from the Panopto embedded iframe within Canvas.

Extension must detect when it’s on a Panopto video page within Canvas environment.

Needs fallback handling if transcripts are unavailable or permission-locked.

Possible future features: highlight-to-prompt, chapter-based extraction, sentiment tagging.

## References & Inspiration

YouTube summarizer extensions like Eightify or Glasp

Liam Kearnan's idea about canvas data extractor
