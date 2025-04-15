# Chrome Extension Idea: PromptMate

## Authors

Sean Donovan

## Problem Statement

ChatGPT users often struggle with crafting effective prompts for large language models. Common pain points include not knowing how to phrase prompts for different content types, spending time manually copying data from various sources, and difficulty in formatting prompts to get consistent, high-quality responses from LLMs. Many users also find that generic prompt templates don't address their specific professional needs, forcing them to spend extra time customizing prompts. PromptMate addresses these challenges by simplifying prompt creation through intelligent data extraction, providing profession-tailored prompt templates, and leveraging OpenAI's capabilities to generate world-class prompts based on user context.

## Target Audience

The target audience for PromptMate is ChatGPT and other LLM users who regularly interact with these AI tools for various tasks. This includes students researching papers, professionals analyzing job descriptions, developers debugging code, content creators, researchers, business professionals, and general users who want to get better results from their LLM interactions without learning complex prompt engineering techniques. PromptMate particularly benefits users whose work spans multiple domains or who need profession-specific prompt recommendations.

## Description

PromptMate is a Chrome extension that helps users create effective prompts for LLMs like ChatGPT through a personalized onboarding process that identifies the user's profession. It extracts data from web pages and clipboard content, then suggests appropriate prompt templates tailored to both content type and professional context. The extension simplifies prompt creation while ensuring users maintain control, and offers an optional "world-class prompt" feature that generates sophisticated prompts based on clipboard context and professional needs.

## Selling Points

1. Streamlines data extraction from web pages and clipboard, eliminating manual copying and pasting
2. Features profession-based onboarding to personalize the prompt recommendation experience
3. Provides tailored prompt templates that adapt to both content types and professional contexts
4. Maintains user autonomy through editable prompts and flexible profession settings
5. Offers an optional "world-class prompt" feature that leverages OpenAI's capabilities to generate sophisticated, context-aware prompts

## User Stories

1. As a student, I want to extract text from a research paper and get a suitable prompt template, so that I can quickly get a quality summary from ChatGPT.
2. As a developer, I want to format my code snippets with appropriate debugging prompts, so that I can get more accurate troubleshooting assistance from LLMs.
3. As a job seeker, I want to analyze job descriptions with well-structured prompts, so that I can efficiently extract key requirements and match them to my skills.
4. As a casual user, I want simplified prompt creation without learning complex prompt engineering, so that I can get better results from ChatGPT with minimal effort.
5. As a content creator, I want to maintain control over my prompts while getting useful formatting suggestions, so that I can balance guidance with creative autonomy.
6. As a business professional, I want to specify my profession during onboarding, so that I receive prompt suggestions relevant to business analysis and proposal writing.
7. As a researcher, I want prompt templates that understand academic contexts, so that I can get more precise analysis of research papers and data.
8. As a multi-role professional, I want to easily switch between different professional contexts, so that my prompt recommendations adapt to my current task without redoing onboarding.

## Notes

The MVP version of PromptMate enhances the user experience through a profession-based onboarding process that tailors prompt recommendations to specific user needs. During initial setup, users select their profession from a dropdown (e.g., Student, Researcher, Developer, Writer, Business Professional), which informs prompt template customization. This information is stored but remains flexible, allowing users to adjust their profession at any time through settings, ensuring adaptability across varied tasks.

The extension focuses on three key input methods: clipboard content, current web page extraction, and selected text from web pages. These inputs are paired with profession-specific prompt recommendations drawn from OpenAI's understanding of professional language use and public prompt engineering best practices.

For advanced users, a separate "Generate World-Class Prompt" feature analyzes clipboard content and uses the LLM to craft sophisticated prompts tailored to both profession and specific context. This optional feature provides high-quality prompts without requiring users to master prompt engineering themselves.

Future enhancements could include PDF support, OCR for images, automatic content type detection, direct integration with ChatGPT, and further refinement of profession-based recommendations through user feedback.

## References & Inspiration

- [Mozilla Readability GitHub Page for Web Content Extraction](https://github.com/mozilla/readability)
- [OpenAI Best Practices for Prompt Engineering with OpenAI API](https://help.openai.com/en/articles/6654000-best-practices-for-prompt-engineering-with-openai-api)
- [Awesome ChatGPT Prompts - GitHub Repository](https://github.com/f/awesome-chatgpt-prompts)
