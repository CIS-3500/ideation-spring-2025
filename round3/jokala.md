# Chrome Extension Idea: Penn Course GPT Prompt Assistant

## Authors  
- Ioannis Kalaitzidis (jokala)
- Maria Ramos ()
- Claire Zhao ()
- Chaelsey Park (chaelsey)

## Problem Statement  
Students at Penn often struggle with course selection, especially when balancing complex degree requirements, personal interests, and course difficulty. While tools like Path@Penn and Penn Course Review provide information, students still spend a significant amount of time cross-referencing requirement fulfillment, evaluating course fit, and manually composing questions to ask LLMs for recommendations. Our extension eliminates that friction by automatically compiling relevant course options and generating a structured GPT prompt for intelligent, personalized suggestions.

## Target Audience  
The primary users are undergraduate and graduate students at Penn who are planning their semester courses. These students typically navigate degree requirements, seek optimal workload balance, and want to explore courses aligned with their academic and personal interests. The tool is especially helpful to double majors, interdisciplinary students, or those pursuing multiple minors.

## Description  
This Chrome extension integrates with Path@Penn and Penn Course Review to assist in course selection. It extracts outstanding degree requirements, gathers viable course options, and pairs them with difficulty and workload data to generate a personalized GPT prompt. The prompt is ready to copy-paste into any LLM (e.g., ChatGPT, Claude) for informed course selection advice.

## Selling Points  
- Automatically identifies unmet requirements from Path@Penn  
- Gathers difficulty, workload, and rating data from Penn Course Review  
- Allows users to include their academic interests and course history for personalization  
- Generates high-quality, structured GPT prompts to streamline course selection  
- Saves time and reduces cognitive overhead in academic planning  

## User Stories  
1. As a student, I want to extract my remaining requirements from Path@Penn so that I know what categories I need to fulfill.  
2. As a student, I want to see course options that fulfill a specific requirement so that I can plan efficiently.  
3. As a student, I want to view difficulty and workload data for each course so that I can make balanced scheduling decisions.  
4. As a student, I want to input my academic background and interests so that the suggestions are tailored to me.  
5. As a student, I want to generate a GPT-ready prompt with all relevant information so that I can get high-quality course advice instantly.

## Notes  
- We plan to use the Penn Course Review API for course difficulty and workload data.  
- Data from Path@Penn may need to be extracted via DOM parsing due to lack of public APIs.  
- User preferences (e.g., interests, past courses) will be stored locally using Chrome storage.  
- The extension will not directly integrate with GPT to reduce scope, but will generate optimized prompts for user copy-paste.  
- Future versions may include schedule exports, GPT API integration, or recommendation ranking directly in the extension.
