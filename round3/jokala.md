# Chrome Extension Idea: Penn Course GPT Assistant

## Authors
-Ioannis Kalaitzidis, 
- Claire Zhao,
- Maria Ramos,
- Chaelsey Park

## Problem Statement
Penn students often struggle to make informed course decisions, especially when balancing multiple priorities like difficulty, quality, and workload. The original Penn Course Search extension provided fast access to PCR data, but lacked decision support features. Students are left opening multiple tabs, comparing stats manually, and asking peers for help. Our goal was to enhance this experience into an intelligent assistant that helps students pick the right course faster and smarter using GPT and improved visuals.

## Target Audience
- Penn undergraduates during pre-registration or add/drop
- First-years and sophomores trying to explore majors
- Juniors/seniors fulfilling requirements with preferences
- Advisors helping students select courses
- Students who want quick, data-driven class comparisons

## Description
We built this extension as a direct enhancement of the existing [Penn Course Search Chrome Extension](https://github.com/fbc101/PennCourseChromeExtension), created by Franci Branda-Chen, Eshaan Chichula, Matt Fu, and Jake G. Murphy. Their original tool focused on rapid access to PennCourseReview (PCR) data using a sleek Chrome popup and highlight-based search. Our goal was to retain their thoughtful design and expand it into a decision-making assistant for course selection—leveraging GPT for insights, improved visualizations, and new UI flows.
The Penn Course GPT Assistant transforms the original lookup tool into a full-featured Chrome extension that helps you search, compare, and select Penn courses more efficiently. It integrates with the PennCourseReview API and adds OpenAI GPT capabilities to provide course summaries, recommendations, and comparisons—all within a single interface. Students can visually compare courses, store selections, and ask GPT for smart advice with one click.

## Selling Points
1. **Smart GPT Recommendations**: Ask ChatGPT which course to take based on real ratings and workload.
2. **Persistent Course Selections**: Save and compare multiple classes across sessions with checkboxes.
3. **Radar Graph Comparison**: Visualize courses side-by-side using radar charts.
4. **Single Course GPT Summary**: Get a personalized breakdown of a course’s style, rigor, and audience.
5. **Tabular Metric Comparison**: View course stats clearly in table format, with visual badges.
6. **OpenAI Key Management**: Securely store your own API key—no backend required.
7. **Responsive Popup UI**: Mobile-aware, resizable popup interface with tabs and collapsibles.
8. **Error-Handled UI**: Graceful messages if a course is missing data or GPT key isn’t set.
9. **Markdown-to-HTML Rendering**: GPT responses appear styled with bullet points and headings.
10. **Guided UX**: Captions, tooltips, and validation rules help users take correct actions.

## User Stories
1. As a student, I want to compare CIS 1200 and CIS 1600 visually so I can pick based on difficulty.
2. As a user, I want to search by course ID so that I can quickly view course stats without opening Penn InTouch.
3. As a user, I want the extension to detect highlighted text with course codes so I can look up courses in-context.
4. As a user, I want to save selected courses and come back to them later so I can iteratively build my schedule.
5. As a student with limited time, I want GPT to tell me which of my 3 options is objectively better.
6. As a user, I want to toggle between radar and table view to understand stats visually or numerically.
7. As a student, I want to generate a course summary with GPT so I can know if it fits my learning style.
8. As a user, I want helpful error messages when I forget to select courses so that I don’t feel lost.
9. As a user, I want the GPT buttons to be disabled unless conditions are met so that the UI feels polished.
10. As a student, I want to see rating trends across semesters to avoid courses that are in decline.
11. As a user, I want a clean interface that groups current vs. previously selected courses.
12. As a GPT user, I want to store my API key securely so I can use the AI features without entering it every time.
13. As a student, I want to ask GPT for the easier course between two hard ones.
14. As a user, I want to see exactly what GPT was asked so I can trust the recommendation.
15. As a student, I want to remove a previously selected course if I change my mind.
16. As a user, I want to see visual indicators (stars, color) for best/worst course stats.
17. As a user, I want GPT summaries formatted cleanly so I don’t get a wall of text.
18. As a student, I want to compare SSH electives in one click rather than open five browser tabs.
19. As a user, I want tooltips that explain what each rating means.
20. As a user, I want the extension to never send data anywhere except OpenAI (if enabled) so I can feel safe.

## Notes
- We did not modify the original search or highlight lookup logic, but improved all subsequent user flows.
- Our radar chart and GPT response renderer are new React components built on top of the existing App.tsx logic.
- The GPT buttons are conditionally rendered and follow strict validation.
- We took care not to overload the original UX, grouping all AI interactions at the bottom.
- The extension is optimized for performance, only calling GPT when explicitly triggered.

## References & Inspiration
- Original PennCourseChromeExtension: https://github.com/fbc101/PennCourseChromeExtension
- PennCourseReview API Docs: https://penncoursereview.com/api/documentation/
- OpenAI GPT-4o API: https://platform.openai.com/docs
- Inspiration from academic advising experiences and course-planning Reddit threads
