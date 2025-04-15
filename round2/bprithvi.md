# Chrome Extension Idea: AutoAvail for GCal

## Authors  
Prithvi 

## Problem Statement  
Scheduling meetings via email is a tedious and error-prone process because users must manually check their Google Calendar and type out their available times. This inefficiency wastes time and can lead to scheduling conflicts if the calendar data becomes outdated during email composition. The AutoAvail for GCal Chrome extension solves this by integrating with Google Calendar to automatically extract and insert available time slots directly into emails when the user types "{availability}", streamlining the scheduling process.

## Target Audience  
The target audience includes professionals such as salespeople, consultants, project managers, and other individuals who frequently schedule meetings via email and rely on Google Calendar for time management. These users typically compose emails in a browser (e.g., Gmail in Chrome) and need a quick, accurate way to share their availability with others. They value productivity tools that integrate seamlessly into their existing workflows.

## Description  
AutoAvail for GCal is a Chrome extension that enhances email communication by integrating with Google Calendar to suggest available meeting times. When a user types "{availability}" while composing an email, the extension instantly retrieves their free time slots from their calendar and inserts them into the message. It also offers customizable settings, such as restricting availability to 9 AM - 5 PM on weekdays, ensuring users share only their preferred time windows.

## Selling Points  
- **Time-saving**: Automates the process of checking and listing available times, reducing manual effort.  
- **Accuracy**: Pulls real-time data from Google Calendar to prevent scheduling errors or double-bookings.  
- **Convenience**: Seamlessly integrates into the email composition flow with a simple trigger word.  
- **Customizable**: Lets users define availability preferences, like 9-5 on weekdays, to match their work habits.  
- **Productivity boost**: Speeds up meeting coordination, allowing users to focus on their core tasks.

## User Stories  
- As a sales representative, I want to quickly share my available times in client emails so that I can book meetings faster and close deals more efficiently.  
- As a project manager, I want to provide accurate availability based on my current calendar so that I avoid scheduling conflicts with my team.  
- As a consultant, I want to set my availability to only show 9-5 on weekdays so that I maintain a consistent work-life balance.  
- As a user, I want to type '{availability}' and see my free slots instantly so that I don’t have to switch tabs or disrupt my email workflow.  
- As a busy professional, I want to rely on my Google Calendar integration so that my recipients get up-to-date options without manual updates.
- As a university student reaching out to professors for research opportunities, I want to insert my availability easily so I can schedule meetings professionally and quickly without back-and-forth emails.
- As a student networking for job opportunities, I want to share my available times efficiently when following up with alumni or recruiters so that I appear organized and proactive.
- As a remote team member in a different time zone, I want to auto-insert my availability in my local working hours so my teammates can see when I’m free without doing manual time conversions.
- As a freelancer juggling multiple clients, I want to quickly respond to availability requests so that I can focus on billable work instead of scheduling admin.
- As a team lead managing several projects, I want to limit availability inserts to specific calendars (e.g., work only) so that personal commitments don’t appear in scheduling emails.


## Notes  
- The extension requires authentication with the Google Calendar API to access the user’s calendar data securely.  
- Privacy is a priority: it should only fetch calendar data when "{availability}" is typed, not continuously.  
- It must parse calendar events to identify free slots within user-defined settings (e.g., 9-5, Monday-Friday).  
- A potential challenge is handling time zone differences between the user and email recipients; a future feature could adjust times accordingly.  
- An alternative design could add a toolbar button to insert availability, though the trigger word keeps it hands-free and intuitive.

## References & Inspiration  
- Google Calendar API documentation: https://developers.google.com/calendar  
- Inspired by tools like Calendly, which simplify scheduling but lack direct email integration.  
- Inspired by other chrome extensions for GCal focusing on productivity: https://www.timely.com/blog/best-google-calendar-extensions
