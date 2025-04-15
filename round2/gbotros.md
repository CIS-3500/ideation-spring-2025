# Chrome Extension Idea: Docky (GPT Code Snippets for Documentation)

## Authors

George Botros
Christian Ishimwe
Matthew Yin

## Problem Statement

Developers frequently browse documentation websites to understand how to use libraries, APIs, or frameworks. However, these documentation pages often lack practical, contextual code examples tailored to specific programming languages or complexity levels. This creates a barrier for learners and even experienced developers trying to implement features quickly and fully grasp the docs.

Docky solves this by augmenting any documentation page with AI-generated code snippets. By extracting the relevant content from the current page and allowing the user to input their desired complexity level, the extension provides immediate, tailored examples directly on the site.

## Target Audience

Our target users include:

- Beginner and intermediate developers who benefit from seeing code examples alongside explanations.

- Experienced developers who want quick examples or examples at an altered complexity level.

- Educators and students using documentation as learning material.

- Cross-language developers trying to translate documentation from one programming language to another.

## Description

Docky is a Chrome Extension that enhances documentation pages by extracting content and allowing users to prompt for specific examples. Users can specify the programming language (or it will be contextually inferred if not provided) and difficulty level, and the extension will inject tailored code snippets directly below the relevant section of the documentation. It’s like having a personalized assistant that turns explanations into practice on the spot.

## Selling Points

1. Context-Aware Code Generation: Generates examples based on the content currently on-screen.

1. Language and Complexity Control: Users can specify programming language and example difficulty level.

1. Non-Intrusive UI: Integrates seamlessly into existing documentation layouts without disrupting the reading experience.

1. Time-Saving: Reduces the time spent searching StackOverflow or GitHub for usable examples.

1. Learning-Oriented: Helps reinforce learning by showing practical implementations tailored to the reader’s context.

## User Stories

1. As a beginner developer, I want to see a simple example in Python when reading about a function, so that I can better understand how to use it.

1. As an experienced developer, I want to quickly convert a JavaScript example into TypeScript, so that I can use it in my project.

1. As a student, I want to get beginner-level examples when reading complex documentation, so that I can understand foundational concepts.

1. As a developer working across languages, I want to request examples in a different programming language, so that I can apply them to my current tech stack.

1. As a time-constrained engineer, I want to generate examples in one click, so that I don’t need to leave the documentation page.

1. As a frontend developer, I want to generate browser-compatible examples for different environments (e.g., Chrome, Safari), so that I can ensure cross-browser support.

1. As a technical writer, I want to preview AI-generated code snippets based on my draft documentation, so that I can include more accurate examples in the final version.

1. As a developer learning a new framework, I want to get intermediate examples that build on basic concepts, so that I can gradually increase my understanding without being overwhelmed.

1. As a developer working with APIs, I want to auto-generate examples showing how to call specific endpoints, so that I can test them quickly in tools like Postman or fetch-based scripts.

1. As a team lead, I want my team members to be able to generate standardized code examples with predefined complexity and style, so that our codebase stays consistent during onboarding and documentation review.

## Notes

- Could support a “hover-to-preview” feature for snippets to avoid cluttering the page.

- Initial scoping will focus on major documentation sites (e.g., MDN, React, Python Docs).1

## References & Inspiration
