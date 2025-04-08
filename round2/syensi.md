# Chrome Extension Idea:  One-Click ChatGPT Integration

## Authors

Hanxi Guo, Nick Cirillo

## Problem Statement

- LeetCode problems often include lengthy descriptions, complex sample code, and large test cases. Manually copying and pasting these elements into ChatGPT is time-consuming and error-prone
- Users often struggle to extract specific code lines or test cases from LeetCode’s editor (e.g., "Why does this loop fail?"). Copying fragments without the full problem context forces users to spend extra time re-explaining the scenario to ChatGPT.
- When users ask ChatGPT for help, they must manually explain the problem context (e.g., "This line of code doesn’t work with the third test case"). Without structured input, ChatGPT may misinterpret the request, leading to irrelevant or generic responses.

## Target Audience

- Job Seekers for Software Development Roles
- University student who studying data structure and algorithm
- Coding competition participants

## Description

This Chrome Extension streamlines the process of seeking AI assistance for LeetCode problem-solving by **automatically extracting code, problem descriptions, and test cases** directly from the LeetCode editor. With one click, it structures this data into context-rich prompts and sends them to *ChatGPT*, eliminating manual copy-pasting and fragmented explanations. Its **core purpose** is to turn ChatGPT into a targeted coding assistant that understands both the problem’s constraints and the user’s specific struggles, and saving time for users to learning from code and problems.


## Selling Points

1. **One-Click Extraction** : Automatically extracts code, problem descriptions, and test cases from the LeetCode editor with a single click.
2. **Context Integration**: Integrates problem descriptions, code, and test cases into structured prompts for ChatGPT
3. **Privacy protection**: Data is processed locally to prevent sensitive code or problem leaks to third-party servers.
4. **Multi-language support**: Multi-language is supported by AI, attracting user from diverge background
5. **Multi-Format Support**: Supports exporting data in plain text, Markdown, or JSON formats for compatibility with ChatGPT and other AI tools.

## User Stories
1. **As a job seeker preparing for technical interviews,** I want to speed up on finding the problem of my coding
2. **As a university student struggling with a complex algorithm,**  I want to right-click a confusing code line in the LeetCode editor and know the meaning of them
3. **As a coding competition participant**, I want to quickly clarify why a specific test case failed so that I can efficiently debug and refine my algorithm during competitions.
4. **As a university student learning data structures**, I want a simplified method to discuss complex problem descriptions with ChatGPT so that I can deepen my conceptual understanding faster.
5. **As a software developer refreshing coding skills**, I want instant context-rich ChatGPT prompts based on LeetCode problems so that I can quickly identify mistakes without retyping or summarizing the problem details.
6. **As an interviewee practicing for coding tests**, I want to quickly troubleshoot unexpected runtime errors by highlighting problematic lines, automatically providing context to ChatGPT so I receive precise feedback.
7. **As a coding bootcamp student**, I want automatic extraction of relevant problem details so I can easily follow structured AI guidance and learn coding techniques more efficiently.
8. **As an international user**, I want to effortlessly use ChatGPT with extracted multilingual problem descriptions and test cases to improve my coding skills regardless of language barriers.
9. **As an instructor**, I want students to easily clarify their confusion through structured AI prompts directly from LeetCode problems, improving their independent problem-solving skills.
10. **As a learner focusing on optimization**, I want to quickly ask ChatGPT how to improve my solution’s performance based on the problem constraints and existing code, enabling more targeted practice.

## Notes
- Not sure if leetcode have policy that do not allow extracting problem and testcases

## References & Inspiration
[Leetcode-Questions-Scraper](https://github.com/Bishalsarang/Leetcode-Questions-Scraper)
[Thinking of the use of leetcode in reddit](https://www.reddit.com/r/learnprogramming/comments/19fhawy/why_do_some_software_engineers_say_leetcode_isnt/)
_[Include any references or sources that inspired your Chrome Extension idea. This could be articles, existing products, or other resources that informed your concept. Just paste any links you found during research.]_