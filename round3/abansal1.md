# Chrome Extension Idea: ClassMatch AI

## Authors
Arya Bansal, Maria Ramos

## Problem Statement
When registering for classes at Penn, students often face difficulty choosing between multiple course options that fit with their schedule. They must manually read Penn Course Review data, ask peers, and compare scattered pieces of feedback. This process is time-consuming and subjective. An automated tool to synthesize reviews and suggest courses based on personal preferences would dramatically streamline course selection.

## Target Audience
This application is designed for Penn students selecting courses during registration periods.

## Description
ClassMatch AI integrates with Path@Penn and Penn Course Review to simplify the course selection process. It allows students to choose a set of potential courses and input preferences (e.g., light workload, engaging lectures, helpful professors). The extension then scrapes course evaluation data and returns recommendations on which course aligns best with the user’s preferences.

## Selling Points
- Automatically scrapes and processes Penn Course Review data for selected courses.
- Asks the user for personal preferences and aligns them with quantifiable metrics (difficulty, quality, workload, etc.).
- Offers clear, ranked suggestions for which course to take based on stated preferences.
- Reduces time and stress during registration by eliminating manual review comparisons.
- Provides transparent reasoning for each suggestion (e.g., “You said you prefer lighter workloads. Course X is rated lowest in workload.”).
- Designed to be lightweight and integrated with Path@Penn for seamless access.

## User Stories
- As a student, I want to pull my shortlist of classes from Path@Penn so that I don’t need to manually enter course names.
- As a student, I want to input what I care about in a class (e.g., easy grading, good professor) so that I receive tailored suggestions.
- As a student, I want the extension to fetch and compare Penn Course Review data so that I don’t have to manually read through reviews.
- As a student, I want to receive a ranked recommendation list based on my input preferences so that I can make more informed registration decisions.
- As a student, I want to view a breakdown of why a particular course is recommended so that I can trust the system's decision-making.
- As a student, I want to have the option to adjust my preferences and rerun the comparison so that I can explore different trade-offs.
- As a student, I want an intuitive interface that guides me step-by-step through comparison and review so that I don’t feel overwhelmed.
- As a student, I want to ensure that my selected courses and preferences are saved temporarily so that I can revisit them before finalizing registration.
- As a student, I want my data to be handled securely without unnecessary collection or sharing so that I can feel safe using the tool.
- As a student, I want an option to export the analysis (e.g., summary PDF or CSV) so that I can consult it offline or share it with advisors.

## Notes
The primary feature will center around fetching user-selected classes from Path@Penn, capturing their class preferences via prompts, and using Penn Course Review data to perform a weighted match. The strength of this application lies in its ability to create a meaningful match between qualitative preferences and quantitative course feedback.

## References & Inspiration
Inspired by course selection tools like Coursicle and Penn Course Alert, but more personalized and intelligent, focusing on maximizing alignment between student preferences and historical feedback.




