## Chrome Extension: Google Scholar Article Search (based on keywords and relevance of abstract)

### Concept
A Chrome extension where users input a topic or keywords, and it searches Google Scholar (or uses cached search results), identifies recently published articles, extracts abstracts using Semantic Scholar API, and uses an LLM to determine which are most relevant.


### Core Features
* Input a search query or keyword list.
* Automatically fetches a set number of recent results from Google Scholar (e.g., published in the past 6–12 months).
* For each abstract, runs LLM summarization and relevance scoring (e.g., "How related is this paper to X?").
* Ranks and displays the top-N most relevant papers with summaries.


### Why it works
* Solves the overload problem: researchers often see too many new papers.
* Uses LLMs intelligently to surface what's actually relevant, not just what's ranked high.
* Creates cleaner, more targeted input for further prompt-based exploration or synthesis.


### Bonus Ideas
* Allow exporting selected summaries into a markdown/CSV file.
* Add a “notify me weekly” option to check for updates on a given topic.


This project proposes the development of a Chrome extension designed to help researchers efficiently discover new, high-relevance academic articles on topics they care about. The extension will allow users to input a search query or list of keywords and will automatically fetch recent Google Scholar results (for example, articles published within the past 6 to 12 months). For each article retrieved, the extension will extract the abstract and use a large language model (LLM) to summarize the content and assess its relevance to the user's specified topic.

By combining summarization with semantic relevance scoring, the tool will present a ranked list of the most pertinent new papers, streamlining the research process and helping users quickly focus on high-value content. The summaries and relevance indicators will appear in a clean, user-friendly interface within the browser, with optional features such as the ability to export summaries to CSV/Markdown, or receive weekly update notifications for specific topics.

This project directly supports the semester’s theme of streamlining and accelerating the extraction of input data for LLM prompt generation. By narrowing down the overwhelming volume of newly published academic literature and summarizing it into digestible, contextually relevant chunks, the extension enables faster, smarter use of LLMs for downstream tasks like literature reviews, prompt generation, and research synthesis.


## USER STORIES

1. As a user, I want to input a custom search query or keywords, so I can tailor the article results to my specific research interests.
2. As a user, I want each article’s abstract to be summarized by an LLM, so I can quickly understand the key points without reading the full abstract.
3. As a user, I want the system to score and rank each article based on how relevant it is to my query, so I can focus on the most relevant ones first.
4. As a user, I want to filter results by publication date range, so I can focus on the most recent or relevant time window.
5. As a user, I want to click a button to view the full article or PDF link when available, so I can dive deeper into the papers I’m most interested in.
6. As a user, I want to see a clean, scrollable list of summarized articles within the extension, so I can review results without leaving the current page.
7. As a user, I want to manually mark articles as ‘relevant’ or ‘not relevant,’ so the system can improve future recommendations based on my preferences.
8. As a user, I want to see a loading or progress indicator during summarization and relevance scoring, so I know the extension is working and not stalled.
9. As a user, I want to adjust the number of articles fetched per query, so I can control how broad or narrow my results set is.
10. As a user, I want to save individual article summaries with personal notes, so I can keep track of why a paper was important to me.
