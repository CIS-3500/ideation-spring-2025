# Chrome Extension Idea: **MapReviews**

## Authors  
Carson Fisher (carsonf)

## Problem Statement  
Google Maps reviews for restaurants, attractions, and businesses can number in the thousands, making it overwhelming and time-consuming to read through them all. While AI could summarize them effectively, there is currently no easy way to copy or compile even a reasonable number of reviews from a Google Maps location. This extension will solve that problem by allowing users to extract a limited set of visible reviews from a business page in a clean, copyable format.

## Target Audience  
- People exploring new restaurants, stores, or local businesses via Google Maps  
- Tourists planning their itineraries based on local reviews  
- Busy people who want quick insights without reading hundreds of reviews  
- Anyone who values community feedback when choosing where to go

## Description  
This Chrome extension integrates with **Google Maps** and enables users to **extract the first 20–50 visible reviews** for a selected location with a single click. The reviews are pulled directly from the page using DOM manipulation, formatted cleanly, and displayed in a popup or sidebar for quick copying. Users can then paste them into a chatbot like ChatGPT for summarization. The extension is fully client-side and does not require backend infrastructure or use of the Google Maps API.

## Selling Points  
1. **Saves time** by avoiding the need to scroll and read dozens of reviews  
2. **Saves Reading** by letting users quickly summarize reviews using AI  
3. **Consistent Formatting** makes raw reviews easier to process or scan manually  
4. **Supports informed decisions**, especially in new or unfamiliar locations  

## User Stories  
- As a traveler, I want to quickly understand if a local spot is worth visiting based on community reviews, so I can make the most of my trip.  
- As a busy student, I want to copy reviews into ChatGPT to summarize them and decide whether a place is worth checking out.  
- As a person with dietary restrictions, I want to easily search for keywords in reviews, so I can avoid surprises.  
- As someone who leaves reviews, I want my contributions to be easier for others to access and summarize.

## Notes  
This version limits review scraping to a feasible number (e.g., 20–50) to avoid needing to scroll infinitely or manage pagination. The extension uses JavaScript to scroll the review container, extract visible reviews, and show them in a simple popup or new tab. It does not require interaction with Google’s API and is scoped to desktop only.

## References & Inspiration  
Inspired by the Recipe extension but with the same structure applied to Google Maps. Designed to be feasible for a third-year computer science student using content scripts, manifest v3, and basic frontend JavaScript.
