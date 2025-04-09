# Chrome Extension Idea: Academic Research Extractor

## Authors
Arya Bansal

## Problem Statement
Academic research often requires efficiently extracting information from research papers to use with LLMs for analysis, summarization, or citation. Currently, researchers and students must manually copy-paste content from papers across multiple tabs, which is time-consuming and disrupts workflow. Extracting structured information (like abstracts, methods, results) and maintaining proper formatting is particularly tedious. Our extension eliminates this friction by automatically detecting and extracting metadata and content from research papers for seamless use with LLMs.

## Target Audience
The primary target audience consists of:
- Academic researchers and graduate students who regularly read and analyze scientific papers
- Undergraduate students working on research projects and literature reviews
- Professors and teaching assistants who need to evaluate or explain research papers
- Knowledge workers who need to stay current with academic literature in their field

These users typically have intermediate to advanced digital literacy, value efficiency, and are already using LLMs to assist with their research workflow.

## Description
Academic Research Extractor automatically detects and extracts structured metadata and content from research papers on sites like arXiv, Google Scholar, Semantic Scholar, and publisher websites. With a single click, users can capture title, authors, abstract, methodology, results, and references, then send this structured information directly to their preferred LLM with customized prompts for specific research tasks.

## Selling Points
1. **Save Time**: Eliminate tedious manual copying and formatting of research papers, reducing a multi-minute process to a single click.
2. **Structured Extraction**: Intelligently separates papers into meaningful sections (abstract, methods, results, references) rather than extracting everything as one block of text.
3. **Built-in Prompt Templates**: Includes research-optimized prompt templates for common tasks like summarization, explanation of methods, or identifying key findings.
4. **Citation Generation**: Automatically formats bibliography entries in multiple styles (APA, MLA, Chicago, BibTeX) for easy reference management.
5. **Wide Platform Support**: Works across major research platforms including arXiv, Google Scholar, PubMed, IEEE Xplore, and many academic publisher websites.

## User Stories
1. As a graduate student, I want to extract the methodology section from a research paper so that I can ask an LLM to explain complex statistical techniques in simpler terms.
2. As a researcher, I want to automatically generate properly formatted citations for papers I'm reading so that I can easily add them to my bibliography without manual formatting.
3. As a professor, I want to extract key findings from multiple papers so that I can ask an LLM to compare and contrast their approaches and results.
4. As an undergraduate student, I want to extract technical abstracts so that I can ask an LLM to explain them in simpler language that I can understand.
5. As a researcher, I want to extract references from papers I'm reading so that I can quickly identify other relevant papers for my literature review.
6. As a teaching assistant, I want to extract mathematical formulas from research papers so that I can ask an LLM to explain their application in course-relevant contexts.
7. As a non-native English speaker, I want to extract complex academic writing so that I can ask an LLM to simplify the language while preserving the meaning.
8. As a researcher conducting a literature review, I want to extract multiple paper abstracts in one session so that I can ask an LLM to identify common themes and gaps.
9. As a graduate student, I want to save extracted paper content to my personal database so that I can build a searchable library of relevant research.
10. As an interdisciplinary researcher, I want to extract domain-specific terminology from papers so that I can ask an LLM to explain unfamiliar concepts from other fields.

## Notes
- Parsing PDFs directly may present technical challenges, so initial implementation might focus on HTML/text-based sources like arXiv, open access journals, and repository sites.
- Different publishers structure their pages differently, requiring customized extraction logic per site.
- Academic papers often contain mathematical formulas, tables, and figures that may require special handling.
- We should consider privacy concerns around sending academic content to third-party LLMs.
- Future versions could integrate with reference management software like Zotero or Mendeley.
- We might need to incorporate OCR capabilities for extracting text from papers available only as scanned PDFs.

## References & Inspiration
- ArXiv API: https://arxiv.org/help/api
- Semantic Scholar API: https://www.semanticscholar.org/product/api
- OpenAlex API: https://docs.openalex.org/
- Crossref API: https://www.crossref.org/documentation/retrieve-metadata/rest-api/
- Zotero: https://www.zotero.org/support/dev/web_api/v3
- Google Scholar: https://scholar.google.com/
- ResearchRabbit: https://www.researchrabbit.ai/
- Elicit: https://elicit.org/
- Connected Papers: https://www.connectedpapers.com/
- SciHub: https://sci-hub.se/
