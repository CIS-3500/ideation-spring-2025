# Chrome Extension Idea: Hyperlink Research Assistant

## Authors

Sofia Segalla, Sean Fang, Jaime Walter Perez, and Daniyah Hasan

## Problem Statement

When copying text to ChatGPT, only copies text but does not copy the hyperlinks that go beneath texts or buttons. We want to have a button that easily does that, and be flexible with multiple use cases.

## Target Audience

We are targeting individuals who would like to conduct deep research on a particular topic. Specifically, this tool is targeted at individuals who may need to learn a great deal or conduct a lot of research within a topic. Having the ability to move between links and explore relationships between content within a page and the links along with content within the links will help create a better picture of the desired topic for a user.

## Description
We’re building a relatively simple but surprisingly useful Chrome extension that lets you instantly copy all the hyperlinks from whatever webpage you’re on—whether that’s Wikipedia, a blog, or a research article. Normally, when you copy text from a page, you lose the actual links hidden behind the words, which makes collecting sources or references kind of a pain. This extension solves that by grabbing every hyperlink (using the standard `<h ref>` tags) with just one click. You can then paste them wherever you want, whether that’s into a database, a research doc, or a citation manager. To take this extension to the next level, we are adding optional predefined prompts that help you do things like figure out which links are relevant to a topic you’re researching, or automatically format them in Chicago style. Users can choose from existing prompts such as:
* "Which of these links are most relevant to my research topic?"
* "Format these links in Chicago style for a bibliography."
* "Identify any links that might contain information on [your topic]."
The goal is to improve the ease with which users can use ChatGPT to help with their research. In many cases, Wikipedia provides interesting content, but you need to follow the footnotes in order to get deeper into the topic. Our extension will follow these links and summarize them for you. 

## Selling Points
1. **Instant Link-Extraction:** Use one button to instantly capture all the links on a given page
2. **Preservation of Information:** Allows LLMs to see the exact context that a user sees without stripping crucial links or hypertext data.
3. **AI-Powered Research Filtering:** Leverage built-in prompts from our extension to automatically identify which links are most relevant to your specific research topics.
4. **Simplified Knowledge Grouping:** Create comprehensive resource collections with minimal effort, supporting more thorough and well-documented research.
5. **Automated Citation Formatting:** Transform raw links into properly formatted citations in Chicago style (with potential for additional citation styles).

## User Stories

* As a researcher, I want to be able to quickly examine all the references of the page I am currently in to know what could be relevant to visit next.
* As a person looking for jobs, I want to be able to copy all the email addresses in a page to make a list of emails to send cold emails.
* As I am learning to use a website, I want to be able to copy all links behind buttons, feed them to ChatGPT and ask it which button I should press to take me to a specific page.
* As a student, I want to be able to quickly extract all the references in a scholarly page and feed them to ChatGPT to quickly make APA style references.
* As a content manager, I want to scan all outbound links from our company’s website to ensure they’re still live and don’t lead to 404 pages.
* As a software engineer, I want to extract all documentation and API links from a GitHub README so I can organize my onboarding notes.
* As an investigative journalist, I want to extract all links from a corporate press release page so I can trace and verify claims with primary sources before publishing, without missing any hidden links that are not highlighted.
* As a customer, I want to extract all the links from Amazon to make a list of products that appeared in my search.
* As a philosophy major, I want to gather all Stanford Encyclopedia of Philosophy links on a topic to understand its conceptual history.
* As a physics major, I want to feed all CERN links on a page into ChatGPT and ask which are best for beginners.
*As a thesis writer, I want to extract all footnote links from academic articles to build a comprehensive bibliography without manually formatting each citation.
* As a data journalist, I want to gather all source links from government reports to verify claims and cross-reference statistics before publishing my analysis.
* As a fact-checker, I want to grab all links from a news article to quickly assess the credibility of sources and identify potential bias.
* As a historian, I want to extract links from archival websites to create a chronological map of primary sources related to my research period.
* As a literature reviewer, I want to collect all citation links from multiple papers in my field to identify recurring references and seminal works.




## Notes

**Potential Challenges/Limitations:**
* Some sites load content (and links) dynamically with JavaScript, so it will be very hard to find these links with simple scraping techniques, and the extension may not work on some specific websites. 
* We may want to filter noise– some pages have hundreds of links, many of which can be redundant (like ads or duplicate links). 
* We also need to be conscious of malformed links


## References & Inspiration

We wanted to utilize these LLMs for deep research and reading efficiency. The one place we all struggled with was keeping track of references in our pages and ensuring that all linked context was fully given to the LLM for maximum accuracy. So our original idea was to extract content from links, but we came to the idea of actually finding links, grouping relevant links, and generating link context because we believe this will be the biggest help in research.
