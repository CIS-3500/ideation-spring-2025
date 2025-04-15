# Chrome Extension Idea: LinkedIn Job Snatcher

A Chrome extension that, when the user is on LinkedIn, copies the current job description on the page into their clipboard and automatically opens ChatGPT, pasting the job description into the input box for easy interaction.

## Authors  
Nilla Orina, Aaron Jiang, Tommy Li

## Problem Statement  
When browsing job listings on LinkedIn, users often want to analyze or customize their resumes or cover letters using tools like ChatGPT. However, manually selecting, copying, and cleaning up job descriptions from LinkedIn can be tedious. This extension streamlines that process, saving time and reducing friction for users who rely on AI to assist with job applications.

## Target Audience  
This extension is designed for job seekers, particularly students, recent graduates, and professionals who use AI tools like ChatGPT to craft tailored applications. Many of these users are already active on LinkedIn and apply to multiple jobs daily. Career coaches who optimize job application workflows will also benefit.

## Description  
This Chrome extension detects when a user is on a LinkedIn job posting page. With one click, the extension extracts the full job description, copies it to the clipboard, and then opens ChatGPT in a new tab. Upon loading, the extension automatically pastes the job description into the input box so users can immediately begin working on their prompt without needing to copy and paste manually. The extension also has preset prompts to compare a job description with your skill set or resume (pasted via textbox). Built with Manifest V3 for improved performance and security, the extension integrates seamlessly with users’ AI-assisted workflows like resume tailoring or job description summarization.

## Selling Points  
1. One-click job description copy and auto-paste into ChatGPT for quick interaction with AI tools.  
2. Automatically recognizes LinkedIn job post pages – no need to manually highlight text.  
3. Cleans formatting to ensure pasted text is structured and readable.  
4. Lightweight and fast, with no external dependencies or API calls.  
5. Perfect for job seekers using AI, especially those applying to many positions quickly.

## User Stories  

1. As a job seeker, I want to copy the job description with one click and have it automatically loaded into ChatGPT so that I can start tailoring my resume without hassle.  
2. As a student applying for internships, I want a fast way to grab job details and instantly load them into ChatGPT to help customize my application.  
3. As a career coach, I want to help my clients streamline their job application process by providing a seamless way to work with AI tools.  
4. As a LinkedIn user, I want to avoid manually highlighting and copying job text so I can stay in flow while browsing.  
5. As a ChatGPT user, I want to quickly extract job descriptions and see them already loaded in the input box so I can immediately start editing.
6. As a job seeker, I want to choose from different prompt templates so that I can generate a resume rewrite, cover letter, or skills comparison based on the job description.
7. As someone unfamiliar with ChatGPT prompts, I want the extension to include default prompts so that I get better AI results without needing to write anything myself.
8. As a power user, I want the ability to save and reuse my own custom prompts so that I can maintain consistency in my job applications.
9. As a multitasker, I want the extension to show a confirmation message when the job description and prompt are copied so I know the action worked.
10. As a user applying to many jobs quickly, I want to copy and reuse prompts across listings so that I can keep my workflow fast and efficient.

## Notes  
- Will need to ensure the extension only activates on valid LinkedIn job post URLs.   
- Potential to expand to other job sites like Indeed or Handshake in the future.

## References & Inspiration  
- https://www.linkedin.com/feed/
- https://www.rezi.ai/posts/chatgpt-resume


